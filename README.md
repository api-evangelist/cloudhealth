# CloudHealth (cloudhealth)

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
