# Consul Connect (consul-connect)

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
