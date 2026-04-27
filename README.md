# CloudHealth (cloudhealth)

CloudHealth (now VMware Tanzu CloudHealth, owned by Broadcom) is a multi-cloud financial and operational management platform. It provides cost visibility, optimization recommendations, asset inventory, perspectives (custom groupings), policies, governance, tagging, metrics, and partner/MSP billing workflows across AWS, Azure, GCP, Oracle, and data center environments. Programmatic access is offered through both a REST API at `chapi.cloudhealthtech.com` and a GraphQL API exposed in the platform UI under Setup > Admin > GraphQL Explorer.

**APIs.json:** [apis.yml](https://raw.githubusercontent.com/api-evangelist/cloudhealth/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **x-type:** company
- **Company:** Broadcom (formerly VMware / Tanzu)
- **Position:** Consumer
- **Access:** 3rd-Party

## Tags

Cloud Cost, Cloud Governance, Cloud Management, Cost Optimization, FinOps, Multi-Cloud

## APIs

### CloudHealth REST API
REST API at `https://chapi.cloudhealthtech.com` for managing AWS/Azure accounts, generating OLAP cost and usage reports, querying assets, managing perspectives (groupings), tagging, metrics ingest/query, policies, and partner-tenant provisioning. Authentication uses Bearer tokens issued from the CloudHealth UI.

- [Documentation](https://apidocs.cloudhealthtech.com/)
- [Authentication](https://apidocs.cloudhealthtech.com/#documentation_authenticating-api-requests)

### CloudHealth GraphQL API
GraphQL API exposed in the CloudHealth UI under Setup > Admin > GraphQL Explorer for programmatic interaction with the platform's reporting and asset model.

- [Documentation](https://apidocs.cloudhealthtech.com/)

### CloudHealth Partner API
Partner-specific REST endpoints for MSPs to provision customers, assign AWS/Azure accounts, manage custom price books, billing rules, and customer statements at scale.

- [Documentation](https://apidocs.cloudhealthtech.com/#partner)

## Common Properties

- [Website](https://www.vmware.com/products/cloud-infrastructure/tanzu-cloudhealth)
- [Documentation](https://apidocs.cloudhealthtech.com/)
- [Product Documentation](https://techdocs.broadcom.com/us/en/vmware-tanzu/cloudhealth/tanzu-cloudhealth/saas/tnz-cloudhealth/index.html)
- [Authentication](https://apidocs.cloudhealthtech.com/#documentation_authenticating-api-requests)
- [JSON-LD](json-ld/cloudhealth-context.jsonld)
- [Spectral](rules/cloudhealth-rules.yml)
- [Naftiko Capabilities](capabilities/cloudhealth-capabilities.yml)

## Maintainers

- **FN:** Kin Lane
- **Email:** kinlane@gmail.com
