# Consul Connect (consul-connect)

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

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/consul-connect/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/consul-connect/refs/heads/main/apis.yml)

## Tags

- Consul
- Envoy
- HashiCorp
- Intentions
- Kubernetes
- mTLS
- Service Mesh
- Sidecar
- Zero Trust

## Timestamps

- **Created:** 2025-01-01
- **Modified:** 2026-05-19

## APIs

### Consul Connect HTTP API

The HTTP API exposed by Consul agents under /v1/connect for managing intentions, the Connect certificate authority, and related mesh operations. Connect-related endpoints also exist in the Agent and Catalog APIs for sidecar proxy registration and CA leaf signing.

- **Human URL:** [https://developer.hashicorp.com/consul/api-docs/connect](https://developer.hashicorp.com/consul/api-docs/connect)
- **Base URL:** `http://localhost:8500/v1`

#### Tags

- HTTP API
- Intentions
- mTLS
- Service Mesh

#### Properties

- [Documentation](https://developer.hashicorp.com/consul/api-docs/connect)
- [Reference](https://developer.hashicorp.com/consul/api-docs/connect/intentions)
- [Reference](https://developer.hashicorp.com/consul/api-docs/connect/ca)
- [OpenAPI](openapi/consul-connect-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/consul-connect.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/consul-connect.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/consul-connect-intention-schema.json) — [JSON Schema](https://json-schema.org/specification)

### Consul Connect Configuration Entries

Consul Connect configuration entries (service-defaults, service-resolver, service-router, service-splitter, service-intentions, mesh, proxy-defaults) that declaratively configure mesh behavior. Configuration entries are managed via the /v1/config API and via Kubernetes Custom Resource Definitions when running on Kubernetes.

- **Human URL:** [https://developer.hashicorp.com/consul/docs/connect/config-entries](https://developer.hashicorp.com/consul/docs/connect/config-entries)
- **Base URL:** `https://developer.hashicorp.com`

#### Tags

- Configuration Entries
- CRD
- Kubernetes
- L7 Routing

#### Properties

- [Documentation](https://developer.hashicorp.com/consul/docs/connect/config-entries)
- [Reference](https://developer.hashicorp.com/consul/docs/connect/config-entries/service-defaults)
- [Reference](https://developer.hashicorp.com/consul/docs/connect/config-entries/service-router)
- [Reference](https://developer.hashicorp.com/consul/docs/connect/config-entries/service-splitter)
- [Postman Collection](collections/consul-connect.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/consul-connect.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Consul Connect Gateways

Consul Connect supports four gateway types for traffic flowing into and out of the mesh: mesh gateways for cross-datacenter and cross-partition traffic, ingress gateways for North-South entry, terminating gateways for access to non-mesh services, and the Consul API Gateway implementing the Kubernetes Gateway API.

- **Human URL:** [https://developer.hashicorp.com/consul/docs/connect/gateways](https://developer.hashicorp.com/consul/docs/connect/gateways)
- **Base URL:** `https://developer.hashicorp.com`

#### Tags

- API Gateway
- Gateways
- Ingress
- Mesh Gateway
- Terminating Gateway

#### Properties

- [Documentation](https://developer.hashicorp.com/consul/docs/connect/gateways)
- [Reference](https://developer.hashicorp.com/consul/docs/connect/gateways/mesh-gateway)
- [Reference](https://developer.hashicorp.com/consul/docs/connect/gateways/ingress-gateway)
- [Reference](https://developer.hashicorp.com/consul/docs/connect/gateways/terminating-gateway)
- [Reference](https://developer.hashicorp.com/consul/docs/api-gateway)
- [Postman Collection](collections/consul-connect.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/consul-connect.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Website](https://www.consul.io/)
- [JSON-LD](json-ld/consul-connect-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [JSON Schema](json-schema/consul-connect-intention-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Vocabulary](vocabulary/consul-connect-vocabulary.yml)
- [Spectral Rules](rules/consul-connect-rules.yml)
- [Capability](capabilities/manage-service-intentions.yml)
- [Capability](capabilities/rotate-mesh-ca.yml)
- [Documentation](https://developer.hashicorp.com/consul/docs/connect)
- [Documentation](https://developer.hashicorp.com/consul/api-docs/connect)
- [GitHub Repository](https://github.com/hashicorp/consul)
- [GitHub Organization](https://github.com/hashicorp)
- [Issue  Tracker](https://github.com/hashicorp/consul/issues)
- [Changelog](https://github.com/hashicorp/consul/releases)
- [License](https://github.com/hashicorp/consul/blob/main/LICENSE)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
