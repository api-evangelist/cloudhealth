---
name: cloudhealth-enable-aws-account
description: Connect an AWS account to CloudHealth, check it, update its credentials and remove it again.
api: cloudhealth:cloudhealth-aws-accounts-api
operations:
  - openapi/cloudhealth-aws-accounts-api-openapi.yml#enableAwsAccount
  - openapi/cloudhealth-aws-accounts-api-openapi.yml#getAwsAccount
  - openapi/cloudhealth-aws-accounts-api-openapi.yml#updateAwsAccount
  - openapi/cloudhealth-aws-accounts-api-openapi.yml#listAwsAccounts
  - openapi/cloudhealth-aws-accounts-api-openapi.yml#deleteAwsAccount
generated: '2026-09-16'
method: generated
source: https://apidocs.cloudhealthtech.com/
---

# CloudHealth: enable an AWS account

1. Send `Authorization: Bearer <api_key>` and `Content-Type: application/json` on every write. Without that content type, the API returns `422`.
2. `enableAwsAccount` (`POST /v1/aws_accounts`): send the account `name` and an `authentication` block. For example, use `protocol: assume_role` with `assume_role_arn` and `assume_role_external_id`. Get the external id from CloudHealth for that account (the docs expose `GET /v1/aws_accounts/:id/generate_external_id`). Store the returned id.
3. `getAwsAccount` (`GET /v1/aws_accounts/{id}`): confirm the account and check its status.
4. `updateAwsAccount` (`PUT /v1/aws_accounts/{id}`): rotate the role ARN or external id.
5. `listAwsAccounts`: check the full inventory, paging with `page` / `per_page`.
6. `deleteAwsAccount` (`DELETE /v1/aws_accounts/{id}`) removes the account. The docs describe no undo. The only way back is to run `enableAwsAccount` again, so confirm with a human before you delete.

Rules
- No idempotency key exists. Before retrying a `POST` that failed, call `listAwsAccounts` so you don't create a duplicate account.
- On `429`, back off (30 requests per minute per client on the REST API).
