---
name: Triage Lucent issues
description: List, inspect, and resolve the bugs and UX issues Lucent detects from session replays.
api: openapi/lucent-openapi-original.json
operations: [listIssues, getIssue, updateIssueStatus]
scopes: [read:lucent, write:issues]
---

# Triage Lucent issues

Lucent watches session replays and files issues (bugs / UX problems). This skill walks
through reviewing them and updating their status.

## Auth
- Data API base URL: `https://app.lucenthq.com`
- Send `Authorization: Bearer <luc_api_... | luc_oat_...>`.
- Reading needs `read:lucent`; changing status needs `write:issues`.

## Steps
1. **List open issues** — `GET /api/v1/issues?status=unresolved&limit=25` (`listIssues`). Results are
   ordered `createdAt` desc then `id` desc; page with the `cursor` query param using `nextCursor`.
2. **Inspect one** — `GET /api/v1/issues/{issueId}` (`getIssue`) for `stepsToReplicate`, `aiVerified`,
   `priority`, `sessionCount`, and any linked ticket (`ticketProvider`/`ticketUrl`).
3. **Update status** — `PATCH /api/v1/issues/{issueId}` (`updateIssueStatus`) with a body status of
   `unresolved`, `ticket_created`, `transient`, or `resolved`.

## Rules
- **Idempotent:** setting an issue to its current status returns `200` with the unchanged issue — safe to retry.
- On `429`, honor the `Retry-After` header before retrying.
- `403` means the token lacks `write:issues`; request that scope (or a key created with "Allow issue status updates").
- Errors come back as `{ "error": "<message>" }` (not RFC 9457).
