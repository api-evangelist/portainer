---
name: portainer-webhooks-manage
description: Create, execute, and delete a webhook in Portainer.
api: openapi/portainer-webhooks-api-openapi.yml
operations:
- postWebhooks
- postWebhooksById
- deleteWebhooksById
generated: '2026-10-03'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/portainer-webhooks-api-openapi.yml ; every operationId checked against the contract
---

# portainer-webhooks-manage

Create, execute, and delete a webhook in Portainer.

## Steps

1. 1. `postWebhooks` – requires the request body fields for the webhook definition and the `X-API-KEY` header.
2. 2. `postWebhooksById` – requires the path parameter `id` of the created webhook and the `X-API-KEY` header.
3. 3. `deleteWebhooksById` – requires the path parameter `id` of the webhook to remove and the `X-API-KEY` header.

## Rules

- Authentication: provide the API key in the `X-API-KEY` header (or a JWT in the `Authorization` header).
- No pagination is required for these endpoints.
- No rate‑limit information is defined; exhaustion returns no specific HTTP status.
