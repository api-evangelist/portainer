---
name: portainer-create-user-with-api-key
description: Create a new user, set its password, and generate an API key for the user.
api: openapi/portainer-users-api-openapi.yml
operations:
- UserCreate
- UserUpdatePassword
- UserGenerateAPIKey
generated: '2026-10-03'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/portainer-users-api-openapi.yml ; every operationId checked against the contract
---

# portainer-create-user-with-api-key

Create a new user, set its password, and generate an API key for the user.

## Steps

1. 1. Call `UserCreate` with the required user fields in the request body.
2. 2. Call `UserUpdatePassword` with the user ID returned from step 1 and provide the new password in the request body.
3. 3. Call `UserGenerateAPIKey` with the same user ID to obtain a new API key.

## Rules

- Auth header: include either `X-API-KEY` (ApiKeyAuth) or `Authorization: Bearer <token>` (jwt) on each request.
