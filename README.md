# Consul Connect

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

Consul Connect is the service mesh subsystem of HashiCorp Consul. Connect provides service identity, mTLS, traffic authorization via intentions, and L7 traffic management through Envoy sidecar proxies. Consul Connect ships with a built-in certificate authority that can also be backed by Vault or external PKI, supports mesh, terminating, ingress, and API gateways, and spans virtual machines, Kubernetes, AWS ECS, AWS Lambda, and Nomad runtimes. Operators interact with Connect through the consul CLI, the HTTP API, configuration entries, and Kubernetes Custom Resource Definitions.

**Areas:** Consul · Envoy · HashiCorp · Intentions · Kubernetes · mTLS · Service Mesh · Sidecar · Zero Trust

## Consul Connect on APIs.io

Everything profiled for Consul Connect is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/consul-connect/](https://apis.io/providers/consul-connect/)** — or go straight to one of the APIs or properties below.

### APIs (4)

- [Consul Connect Configuration Entries](https://apis.io/apis/consul-connect/consul-connect-config-entries/) — Consul Connect configuration entries (service-defaults, service-resolver, service-router, service-splitter, service-intentions, mesh, proxy-defaults) that…
- [Consul Connect Gateways](https://apis.io/apis/consul-connect/consul-connect-gateways/) — Consul Connect supports four gateway types for traffic flowing into and out of the mesh: mesh gateways for cross-datacenter and cross-partition traffic,…
- [Consul Connect CA API](https://apis.io/apis/consul-connect/consul-connect-ca-api/) — Certificate authority management
- [Consul Connect Intentions API](https://apis.io/apis/consul-connect/consul-connect-intentions-api/) — Service-to-service traffic authorization

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Consul Connect Agentic Access](https://apis.io/agentic-access/consul-connect/consul-connect-agentic-access/)

#### JSON Schema (1)

The data models the API reads and writes.

- [Consul Connect Intention](https://apis.io/schemas/consul-connect/consul-connect-intention/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Consul Connect Context](https://apis.io/jsonld/consul-connect/consul-connect-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [Consul Connect Service Mesh Vocabulary](https://apis.io/vocabularies/consul-connect/consul-connect-vocabulary/)

#### Collections (3)

Postman and Open Collection request collections.

- [HashiCorp Consul Connect API](https://apis.io/collections/consul-connect/open-consul-connect/)
- [HashiCorp Consul Connect CA API](https://apis.io/collections/consul-connect/open-consul-connect-ca-api/)
- [HashiCorp Consul Connect CA Intentions API](https://apis.io/collections/consul-connect/open-consul-connect-intentions-api/)

#### Governance rules (2)

Spectral rulesets for the provider's contracts.

- [Consul Connect — jsonschema rules](https://apis.io/rules/consul-connect/consul-connect-jsonschema-spectral-rules/)
- [Consul Connect API Rules](https://apis.io/rules/consul-connect/consul-connect-rules/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Consul Connect Authentication](https://apis.io/security/consul-connect/consul-connect-authentication/)
- [Consul Connect Domain Security](https://apis.io/security/consul-connect/consul-connect-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Consul Connect Plans Pricing](https://apis.io/plans/consul-connect/consul-connect-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Consul Connect Rate Limits](https://apis.io/rate-limits/consul-connect/consul-connect-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Consul Connect Finops](https://apis.io/finops/consul-connect/consul-connect-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.consul.io/)
- [Documentation](https://developer.hashicorp.com/consul/docs/connect)
- [Changelog](https://github.com/hashicorp/consul/releases)
- [Blog](https://www.hashicorp.com/blog/feed.xml)
- [GitHub](https://github.com/hashicorp)

## API Evangelist rating

**Kin Score 33.5** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 57.1 |
| Contract quality | 46.3 |
| Contract governance | 27.3 |
| Operational transparency | 26.3 |
| Developer ergonomics | 31.0 |
| Access clarity | 7.9 |

**Agent readiness 17.9** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | — |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 16.7** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/consul-connect/](https://apis.io/providers/consul-connect/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Consul Connect: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/consul-connect/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
