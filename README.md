# Skurail

> Marketplace infrastructure for developers and agents.

Skurail is an open-source layer over marketplace seller APIs. It connects to a shop on
Shopee, TikTok Shop or Lazada, normalizes orders, products, inventory and returns into
one schema, records every change as an event, and exposes the result to developers
through a REST API and SDK, and to agents through an MCP server and an n8n node.

**Status: bootstrapping.** The repository is being set up; nothing here is usable yet.
Follow the commits for progress.

## Planned packages

| Package | What it does |
| --- | --- |
| `@skurail/core` | Database schema, HTTP client, token vault, queue, events, normalization harness |
| `@skurail/connector-shopee` | Shopee Open Platform connector |
| `@skurail/connector-tiktok-shop` | TikTok Shop Partner API connector |
| `@skurail/connector-lazada` | Lazada Open Platform connector (stub) |
| `@skurail/sdk` | Typed client generated from the OpenAPI document |
| `@skurail/mcp` | MCP server exposing the API as tools |
| `n8n-nodes-skurail` | n8n trigger and action nodes |

Apps: `api` (Fastify), `ingest` (webhook receivers), `worker` (processors and poll scheduler), `dashboard` (Next.js).

## License

Apache-2.0. See [LICENSE](LICENSE) and [NOTICE](NOTICE).
