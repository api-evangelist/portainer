---
name: portainer-team-create-and-inspect
description: Create a new team and then retrieve its details.
api: openapi/portainer-teams-api-openapi.yml
operations:
- TeamCreate
- TeamInspect
generated: '2026-10-03'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/portainer-teams-api-openapi.yml ; every operationId checked against the contract
---

# portainer-team-create-and-inspect

Create a new team and then retrieve its details.

## Steps

1. 1. Use `TeamCreate` with the required `X-API-KEY` header (ApiKeyAuth).
2. 2. Use `TeamInspect` with the required `X-API-KEY` header (ApiKeyAuth) and the team ID returned from step 1.

## Rules

- Auth: Include the `X-API-KEY` header for all requests.
- Idempotency: Not applicable for these operations.
- Pagination: Not applicable for these operations.
- Errors: Follow standard HTTP error responses (e.g., 4xx for client errors, 5xx for server errors).
