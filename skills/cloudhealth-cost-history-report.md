---
name: cloudhealth-cost-history-report
description: Pull CloudHealth cost history for a time interval, optionally broken down by a Perspective, and page through AWS accounts to label the results.
api: cloudhealth:cloudhealth-reports-api
operations:
  - openapi/cloudhealth-reports-api-openapi.yml#costHistoryReport
  - openapi/cloudhealth-perspectives-api-openapi.yml#listPerspectives
  - openapi/cloudhealth-aws-accounts-api-openapi.yml#listAwsAccounts
generated: '2026-09-16'
method: generated
source: https://apidocs.cloudhealthtech.com/
---

# CloudHealth: cost history report

1. Authenticate every call to `https://chapi.cloudhealthtech.com` with `Authorization: Bearer <api_key>` and `Accept: application/json`. The key is per-user; results are scoped to the user's organization and role (pass `org_id` to target another organization).
2. Call `listPerspectives` (`GET /v1/perspective_schemas`) when the report should be grouped by a Perspective; note the perspective id.
3. Call `costHistoryReport` (`GET /olap_reports/cost/history`) with `interval` (for example `monthly`) and the `dimensions` / `measures` you need. Keep the URI under 4000 characters.
4. Call `listAwsAccounts` (`GET /v1/aws_accounts`) with `page` / `per_page` (default 30, max 100) to map account ids to names. Keep calling until a page comes back with fewer than `per_page` results.

Rules
- Read-only flow; safe to retry. The REST API allows 30 requests per minute per client. On `429`, back off exponentially before retrying.
- Errors return `{"error": "..."}`: `403` means a bad API key (a newly generated key invalidates the old one), `422` means a malformed input or a missing JSON content type, and `503` means the backend is at capacity.
- See conventions/cloudhealth-conventions.yml and errors/cloudhealth-problem-types.yml.
