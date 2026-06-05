# CloudHealth (cloudhealth)

CloudHealth (now VMware Tanzu CloudHealth, owned by Broadcom) is a multi-cloud financial and operational management platform. It provides cost visibility, optimization recommendations, asset inventory, custom perspectives (groupings), policies, governance, and partner/MSP billing workflows across AWS, Azure, GCP, Oracle, and data center environments. The platform exposes both a REST API and a GraphQL API for programmatic access to reports, assets, accounts, perspectives, tags, metrics, and partner customer provisioning.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/cloudhealth/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/cloudhealth/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Consumer
- **Access:** 3rd-Party

## Tags

- Cloud Cost
- Cloud Governance
- Cloud Management
- Cost Optimization
- FinOps
- Multi-Cloud

## Timestamps

- **Created:** 2026-03-16
- **Modified:** 2026-05-19

## APIs

### CloudHealth REST API

REST API at https://chapi.cloudhealthtech.com for managing AWS/Azure accounts, generating OLAP cost and usage reports, querying assets, managing perspectives (groupings), tagging, metrics ingest/query, policies, and partner-tenant provisioning. Authentication uses Bearer tokens issued from the CloudHealth UI.

- **Human URL:** [https://apidocs.cloudhealthtech.com/](https://apidocs.cloudhealthtech.com/)

#### Tags

- Assets
- Cost Optimization
- Perspectives
- Reports

#### Properties

- [Documentation](https://apidocs.cloudhealthtech.com/)
- [Authentication](https://apidocs.cloudhealthtech.com/#documentation_authenticating-api-requests)
- [OpenAPI](openapi/cloudhealth-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/cloudhealth.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cloudhealth.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### CloudHealth GraphQL API

GraphQL API exposed in the CloudHealth UI under Setup > Admin > GraphQL Explorer for programmatic interaction with the platform's reporting and asset data model.

- **Human URL:** [https://apidocs.cloudhealthtech.com/](https://apidocs.cloudhealthtech.com/)

#### Tags

- GraphQL
- Reports

#### Properties

- [Documentation](https://apidocs.cloudhealthtech.com/)
- [Postman Collection](collections/cloudhealth.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cloudhealth.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### CloudHealth Partner API

Partner-specific REST endpoints for MSPs to provision customers, assign AWS/Azure accounts, manage custom price books, billing rules, and customer statements at scale.

- **Human URL:** [https://apidocs.cloudhealthtech.com/#partner](https://apidocs.cloudhealthtech.com/#partner)

#### Tags

- MSP
- Partner
- Provisioning

#### Properties

- [Documentation](https://apidocs.cloudhealthtech.com/#partner)
- [Postman Collection](collections/cloudhealth.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cloudhealth.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/CloudHealth)
- [LinkedIn](https://www.linkedin.com/company/cloudhealthtech)
- [Website](https://www.vmware.com/products/cloud-infrastructure/tanzu-cloudhealth)
- [Documentation](https://apidocs.cloudhealthtech.com/)
- [Product  Documentation](https://techdocs.broadcom.com/us/en/vmware-tanzu/cloudhealth/tanzu-cloudhealth/saas/tnz-cloudhealth/index.html)
- [Authentication](https://apidocs.cloudhealthtech.com/#documentation_authenticating-api-requests)
- [Privacy Policy](https://www.broadcom.com/company/legal/privacy/policy)
- [JSON-LD](json-ld/cloudhealth-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Spectral Rules](rules/cloudhealth-rules.yml) — [Spectral](https://docs.stoplight.io/docs/spectral)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
