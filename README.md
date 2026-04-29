# Consul Connect

Consul Connect is the service mesh subsystem of HashiCorp Consul. Connect provides service identity, mTLS, traffic authorization via intentions, and L7 traffic management through Envoy sidecar proxies. Consul Connect ships with a built-in certificate authority that can also be backed by Vault or external PKI, supports mesh, terminating, ingress, and API gateways, and spans virtual machines, Kubernetes, AWS ECS, AWS Lambda, and Nomad runtimes.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/consul-connect/refs/heads/main/apis.yml)

## Tags

- Consul, Envoy, HashiCorp, Intentions, Kubernetes, mTLS, Service Mesh, Sidecar, Zero Trust

## Timestamps

- **Created:** 2025-01-01
- **Modified:** 2026-04-28

## APIs

### Consul Connect HTTP API
The HTTP API exposed by Consul agents under /v1/connect for managing intentions, the Connect certificate authority, and related mesh operations.

**Human URL:** [API docs](https://developer.hashicorp.com/consul/api-docs/connect)

#### Tags
- HTTP API, Intentions, mTLS, Service Mesh

#### Properties
- [Documentation](https://developer.hashicorp.com/consul/api-docs/connect)
- [Intentions](https://developer.hashicorp.com/consul/api-docs/connect/intentions)
- [CA](https://developer.hashicorp.com/consul/api-docs/connect/ca)
- [OpenAPI](openapi/consul-connect-openapi.yml)
- [JSONSchema](json-schema/consul-connect-intention-schema.json)

### Consul Connect Configuration Entries
service-defaults, service-resolver, service-router, service-splitter, service-intentions, mesh, and proxy-defaults configuration entries that declaratively configure mesh behavior.

**Human URL:** [Config entries](https://developer.hashicorp.com/consul/docs/connect/config-entries)

#### Tags
- Configuration Entries, CRD, Kubernetes, L7 Routing

### Consul Connect Gateways
Mesh, ingress, terminating, and API gateways for traffic flowing into and out of the mesh.

**Human URL:** [Gateways](https://developer.hashicorp.com/consul/docs/connect/gateways)

#### Tags
- API Gateway, Gateways, Ingress, Mesh Gateway, Terminating Gateway

## Common Properties

- [Website](https://www.consul.io/)
- [JSON-LD](json-ld/consul-connect-context.jsonld)
- [JSONSchema](json-schema/consul-connect-intention-schema.json)
- [Vocabulary](vocabulary/consul-connect-vocabulary.yml)
- [SpectralRules](rules/consul-connect-rules.yml)
- [Capability: Manage intentions](capabilities/manage-service-intentions.yml)
- [Capability: Rotate CA](capabilities/rotate-mesh-ca.yml)
- [Documentation](https://developer.hashicorp.com/consul/docs/connect)
- [API Docs](https://developer.hashicorp.com/consul/api-docs/connect)
- [GitHubRepository](https://github.com/hashicorp/consul)
- [GitHub Organization](https://github.com/hashicorp)
- [Issue Tracker](https://github.com/hashicorp/consul/issues)
- [Change Log](https://github.com/hashicorp/consul/releases)
- [License](https://github.com/hashicorp/consul/blob/main/LICENSE)

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
