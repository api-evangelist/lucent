---
name: Ingest a Lucent session replay
description: Submit a batch of rrweb session-replay events to the Lucent Ingest API.
api: openapi/lucent-openapi-original.json
operations: [sdkReplay]
scopes: []
---

# Ingest a Lucent session replay

The Ingest API accepts rrweb event batches for a single session window. In most apps the
`@lucenthq/sdk` browser package does this for you; this skill covers the raw contract for
server-side or custom integrations.

## Auth
- Ingest base URL: `https://batch-jobs-lucent.onrender.com`
- Public key `luc_pk_...` in the `X-Lucent-Api-Key` header (or `api_key` query param for `sendBeacon`).
- Public keys are **write-only** — safe to embed client-side.

## Steps
1. **Submit a batch** — `POST /api/sdk/replay` (`sdkReplay`) with a `ReplayBatch` body
   (`session`, `user`, `page`, `replay` (rrweb events), `metadata`, `flush`).
2. Set `flush: "final"` on the last batch to dispatch the session for processing immediately;
   otherwise it stays in a `receiving` state until a scheduled finalizer picks it up.
3. Optionally gzip the body and send `Content-Encoding: gzip`.

## Rules
- **Idempotent per `(sessionId, sequence)`** — resubmitting the same batch stores it once. Safe to retry.
- `401` = `Missing API key` or `Invalid or revoked API key`.
- `429` includes `Retry-After` (seconds); back off before retrying. `500` on the ingest side is retryable.
