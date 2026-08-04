# Graphite (graphite-com)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Graphite is a code review platform built on top of GitHub for stacking pull requests, AI code review, and merging at scale. The gt CLI creates and submits stacked PRs, Graphite Agent (Diamond) provides codebase-aware AI review and chat, and a merge queue batches and tests PRs in parallel. Graphite has no standalone public REST API - it integrates through a GitHub App that consumes GitHub webhooks, the gt CLI (authenticated with a Graphite token), the GT MCP server, and label / GitHub-mediated integrations (Slack, Linear, external merge queue).

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/graphite-com/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/graphite-com/refs/heads/main/apis.yml)

## Tags

- Code Review
- Stacked PRs
- Merge Queue
- AI Code Review
- Developer Tools
- GitHub

## Timestamps

- **Created:** 2026-06-20
- **Modified:** 2026-06-20

## APIs

### Graphite GitHub App

Graphite installs as a GitHub App (graphite-app) on an organization to receive GitHub webhooks for real-time updates on CI status, mergeability, and push events, and to call GitHub's APIs with fine-grained permissions and short-lived tokens. GitHub is the only git provider Graphite integrates with; there is no standalone Graphite-hosted REST API.

- **Human URL:** [https://graphite.com/docs/authenticate-with-github-app](https://graphite.com/docs/authenticate-with-github-app)
- **Base URL:** `https://github.com/apps/graphite-app`

#### Tags

- GitHub App
- Webhooks
- Authentication

#### Properties

- [Documentation](https://graphite.com/docs/authenticate-with-github-app)
- [API Reference](https://github.com/marketplace/graphite-dev)
- [OpenAPI](openapi/graphite-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/graphite-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/graphite-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Graphite CLI (gt)

The gt command-line interface creates, stacks, submits, syncs, restacks, and merges pull requests from the terminal. It authenticates with a Graphite auth token (gt auth) and drives Graphite's hosted platform plus GitHub on the user's behalf.

- **Human URL:** [https://graphite.com/docs/cli-overview](https://graphite.com/docs/cli-overview)
- **Base URL:** `https://app.graphite.dev`

#### Tags

- CLI
- Stacked PRs
- Stacking

#### Properties

- [Documentation](https://graphite.com/docs/cli-overview)
- [API Reference](https://graphite.com/docs/command-reference)
- [OpenAPI](openapi/graphite-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/graphite-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/graphite-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Graphite GT MCP Server

GT MCP is a Model Context Protocol server built into the Graphite CLI (gt mcp) that lets AI agents in tools like Cursor and Claude Code automatically break large changes into smaller, reviewable stacked pull requests. It is a local MCP server over the CLI, not a remote HTTP API.

- **Human URL:** [https://graphite.com/docs/gt-mcp](https://graphite.com/docs/gt-mcp)
- **Base URL:** `https://graphite.com/docs/gt-mcp`

#### Tags

- MCP
- Model Context Protocol
- AI Agents

#### Properties

- [Documentation](https://graphite.com/docs/gt-mcp)
- [OpenAPI](openapi/graphite-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/graphite-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/graphite-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Graphite Agent (Diamond) AI Code Review

Graphite Agent (formerly Diamond, now unified with Graphite Chat) is a codebase-aware AI code review agent that comments on pull requests, answers questions, and helps fix and iterate on code. It is triggered on PRs through the Graphite platform and configured via repository settings, not via a public API.

- **Human URL:** [https://graphite.com/docs/ai-reviews](https://graphite.com/docs/ai-reviews)
- **Base URL:** `https://app.graphite.dev`

#### Tags

- AI Code Review
- Diamond
- Code Review

#### Properties

- [Documentation](https://graphite.com/docs/ai-reviews)
- [Documentation](https://graphite.com/docs/ai-review-customization)
- [OpenAPI](openapi/graphite-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/graphite-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/graphite-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Graphite Merge Queue

The Graphite merge queue batches and tests multiple PRs in parallel once they are ready, reducing wait times and merge conflicts. Integration with an external merge queue is label-based and GitHub-mediated rather than exposed as an HTTP API.

- **Human URL:** [https://graphite.com/docs/graphite-merge-queue](https://graphite.com/docs/graphite-merge-queue)
- **Base URL:** `https://app.graphite.dev`

#### Tags

- Merge Queue
- CI
- Automation

#### Properties

- [Documentation](https://graphite.com/docs/graphite-merge-queue)
- [Documentation](https://graphite.com/docs/external-merge-queue-integration)
- [OpenAPI](openapi/graphite-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/graphite-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/graphite-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Graphite Insights

Graphite Insights tracks team engineering velocity (PR throughput, review latency, and related stats) over indexed repositories, surfaced in the Graphite web app. No public analytics API is documented.

- **Human URL:** [https://graphite.com/docs/insights](https://graphite.com/docs/insights)
- **Base URL:** `https://app.graphite.dev`

#### Tags

- Insights
- Analytics
- Engineering Velocity

#### Properties

- [Documentation](https://graphite.com/docs/insights)
- [Documentation](https://graphite.com/docs/insights-stats-definitions)
- [OpenAPI](openapi/graphite-com-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/graphite-com.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/graphite-com.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/withgraphite)
- [LinkedIn](https://www.linkedin.com/company/graphite-dev)
- [Website](https://graphite.dev)
- [Documentation](https://graphite.com/docs)
- [Plans](plans/graphite-com-plans-pricing.yml)
- [Rate Limits](rate-limits/graphite-com-rate-limits.yml)
- [Fin Ops](finops/graphite-com-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
