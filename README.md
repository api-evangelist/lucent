# Lucent

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Lucent is an AI product manager for session replay: it watches user session recordings continuously and automatically detects bugs and UX issues, surfacing them as prioritized, AI-verified issues with reproduction steps, console logs, network activity, and affected-user counts. It ingests rrweb session batches from a lightweight browser SDK (plus React Native and Flutter), imports replays from providers such as PostHog and Sentry, and exposes a REST Data API to read issues, signals, and insights and to update issue status, webhooks for issue events, and a hosted Model Context Protocol (MCP) server so agents like Claude and Cursor can query Lucent data directly. Founded 2025, Y Combinator Winter 2026 batch.

**Areas:** Company · Session Replay · Product Analytics · Bug Detection · Observability · Artificial Intelligence · Developer Tools · MCP · Webhook

## Lucent on APIs.io

Everything profiled for Lucent is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/lucent/](https://apis.io/providers/lucent/)** — or go straight to one of the APIs or properties below.

### APIs (4)

- [Lucent Insights API](https://apis.io/apis/lucent/lucent-insights-api/) — The Insights API from Lucent — 1 operation(s) for insights.
- [Lucent Issues API](https://apis.io/apis/lucent/lucent-issues-api/) — The Issues API from Lucent — 2 operation(s) for issues.
- [Lucent Sdk API](https://apis.io/apis/lucent/lucent-sdk-api/) — The Sdk API from Lucent — 1 operation(s) for sdk.
- [Lucent Signals API](https://apis.io/apis/lucent/lucent-signals-api/) — The Signals API from Lucent — 1 operation(s) for signals.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Arazzo workflows (1)

Multi-step workflows that chain operations into a business task.

- [Lucent — triage and resolve an issue](https://apis.io/arazzos/lucent/lucent-triage-and-resolve/)

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Lucent Webhooks](https://apis.io/asyncapis/lucent/lucent-webhooks-asyncapi/)

#### Event channels (1)

Individual events and webhooks the provider emits.

- [/](https://apis.io/channels/lucent/webhookdeliveries/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [lucent](https://apis.io/servers/lucent/lucent/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Lucent Agentic Access](https://apis.io/agentic-access/lucent/lucent-agentic-access/)

#### Collections (4)

Postman and Open Collection request collections.

- [Lucent Insights API](https://apis.io/collections/lucent/open-lucent-insights-api/)
- [Lucent Insights Issues API](https://apis.io/collections/lucent/open-lucent-issues-api/)
- [Lucent Insights Sdk API](https://apis.io/collections/lucent/open-lucent-sdk-api/)
- [Lucent Insights Signals API](https://apis.io/collections/lucent/open-lucent-signals-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Lucent Openapi Overlay](https://apis.io/overlays/lucent/lucent-openapi-overlay/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Lucent Authentication](https://apis.io/security/lucent/lucent-authentication/)
- [Lucent Domain Security](https://apis.io/security/lucent/lucent-domain-security/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Lucent Scopes](https://apis.io/scopes/lucent/lucent-scopes/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Lucent Plans Pricing](https://apis.io/plans/lucent/lucent-plans-pricing/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://lucenthq.com)
- [Documentation](https://docs.lucenthq.com)
- [Getting started](https://docs.lucenthq.com/quickstart)
- [API reference](https://docs.lucenthq.com/api-reference/introduction)
- [Pricing](https://lucenthq.com/pricing)
- [Sign up](https://app.lucenthq.com/sign-up)
- [Support](https://lucenthq.com/contact)
- [Blog](https://lucenthq.com/blog)
- [Terms of service](https://lucenthq.com/terms)
- [Privacy policy](https://lucenthq.com/privacy)
- [GitHub](https://github.com/lucent-ai)

## API Evangelist rating

**Kin Score 57.1** — strong · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 75.0 |
| Contract quality | 57.4 |
| Contract governance | 18.2 |
| Operational transparency | 10.5 |
| Developer ergonomics | 73.2 |
| Access clarity | 76.3 |

**Agent readiness 59.7** — agent-ready (gated down from agent-native)

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | verified |
| Auth Clarity | served (partial credit) |
| Idempotency | documented (partial credit) |
| Error Semantics | derived (partial credit) |
| OpenAPI Examples | partial |
| Rate Limit Signal | verified |
| Event Surface Described | yes |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | served (partial credit) |
| Protected Resource Metadata | verified |
| Dynamic Client Registration | yes |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | distinct |

**Regulatory alignment 31.8** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/lucent/](https://apis.io/providers/lucent/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Lucent: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/lucent/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
