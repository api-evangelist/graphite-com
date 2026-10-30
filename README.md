# Graphite

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

Graphite is a code review platform built on top of GitHub for stacking pull requests, AI code review, and merging at scale. The gt CLI creates and submits stacked PRs, Graphite Agent (Diamond) provides codebase-aware AI review and chat, and a merge queue batches and tests PRs in parallel. Graphite has no standalone public REST API - it integrates through a GitHub App that consumes GitHub webhooks, the gt CLI (authenticated with a Graphite token), the GT MCP server, and label / GitHub-mediated integrations (Slack, Linear, external merge queue).

**Areas:** Code Review · Stacked PRs · Merge Queue · AI Code Review · Developer Tools · GitHub

## Graphite on APIs.io

Everything profiled for Graphite is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/graphite-com/](https://apis.io/providers/graphite-com/)** — or go straight to one of the APIs or properties below.

### APIs (4)

- [Graphite Authentication API](https://apis.io/apis/graphite-com/graphite-com-authentication-api/) — Graphite CLI authentication with a Graphite auth token.
- [Graphite GitHub App API](https://apis.io/apis/graphite-com/graphite-com-github-app-api/) — GitHub App install and webhook integration entry points.
- [Graphite Merge Queue API](https://apis.io/apis/graphite-com/graphite-com-merge-queue-api/) — Graphite merge queue actions.
- [Graphite Stacks API](https://apis.io/apis/graphite-com/graphite-com-stacks-api/) — Create, submit, sync, and merge stacked pull requests via the gt CLI.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [graphite](https://apis.io/servers/graphite-com/graphite/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Graphite Com Agentic Access](https://apis.io/agentic-access/graphite-com/graphite-com-agentic-access/)

#### Collections (5)

Postman and Open Collection request collections.

- [Graphite Platform](https://apis.io/collections/graphite-com/open-graphite-com/)
- [Graphite Platform Authentication API](https://apis.io/collections/graphite-com/open-graphite-com-authentication-api/)
- [Graphite Platform Authentication GitHub App API](https://apis.io/collections/graphite-com/open-graphite-com-github-app-api/)
- [Graphite Platform Authentication Merge Queue API](https://apis.io/collections/graphite-com/open-graphite-com-merge-queue-api/)
- [Graphite Platform Authentication Stacks API](https://apis.io/collections/graphite-com/open-graphite-com-stacks-api/)

#### Security (4)

Authentication, trust centre, and vulnerability disclosure.

- [Graphite Com Authentication](https://apis.io/security/graphite-com/graphite-com-authentication/)
- [Graphite Com Domain Security](https://apis.io/security/graphite-com/graphite-com-domain-security/)
- [Graphite Com Trust Center](https://apis.io/security/graphite-com/graphite-com-trust-center/)
- [Graphite Com Vulnerability Disclosure](https://apis.io/security/graphite-com/graphite-com-vulnerability-disclosure/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Graphite Com Plans Pricing](https://apis.io/plans/graphite-com/graphite-com-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Graphite Com Rate Limits](https://apis.io/rate-limits/graphite-com/graphite-com-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Graphite Com Finops](https://apis.io/finops/graphite-com/graphite-com-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://graphite.dev)
- [Documentation](https://graphite.com/docs)
- [Getting started](https://graphite.com/docs/get-started)
- [Pricing](https://graphite.com/pricing)
- [Sign up](https://app.graphite.com/signup)
- [Blog](https://graphite.com/blog)
- [Security](https://graphite.com/docs/privacy-and-security)
- [Terms of service](https://graphite.com/terms-of-service)
- [Privacy policy](https://graphite.com/privacy)
- [GitHub](https://github.com/withgraphite)
- [Status](https://status.graphite.com)

## API Evangelist rating

**Kin Score 54.3** — strong · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 71.7 |
| Contract quality | 48.8 |
| Contract governance | 18.2 |
| Operational transparency | 44.7 |
| Developer ergonomics | 69.0 |
| Access clarity | 53.9 |

**Agent readiness 29.7** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | documented (partial credit) |
| Auth Clarity | bearer (partial credit) |
| Idempotency | documented (partial credit) |
| Error Semantics | — |
| OpenAPI Examples | — |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | yes |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | distinct |

**Regulatory alignment 35.3** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/graphite-com/](https://apis.io/providers/graphite-com/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Graphite: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/graphite-com/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
