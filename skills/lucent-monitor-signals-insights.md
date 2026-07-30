---
name: Monitor Lucent signals and insights
description: Read configured Signals (with match counts) and recent AI-generated Insights from Lucent.
api: openapi/lucent-openapi-original.json
operations: [listSignals, listInsights]
scopes: [read:lucent]
---

# Monitor Lucent signals and insights

Signals are saved prompts Lucent matches against sessions; Insights are periodic AI summaries
of product engagement and friction. Both are read-only.

## Auth
- Data API base URL: `https://app.lucenthq.com`, `Authorization: Bearer <token>`, scope `read:lucent`.

## Steps
1. **List signals** — `GET /api/v1/signals?limit=50` (`listSignals`) → each signal's `name`, `prompt`,
   `status`, `matchCount`, and `lastMatchAt`. Default limit 50, max 200.
2. **List insights** — `GET /api/v1/insights?limit=25` (`listInsights`) → recent insights with
   `intervalStart`/`intervalEnd`, `sessionsCount`, and a `contentPreview`. Default limit 25, max 100.
3. **Page** with `cursor` using the `nextCursor` field when present.

## Rules
- Ordered `createdAt` desc, then `id` desc.
- On `429`, wait for `Retry-After` seconds.
- To act on what you find (e.g. resolve a related issue), use the *Triage Lucent issues* skill.
