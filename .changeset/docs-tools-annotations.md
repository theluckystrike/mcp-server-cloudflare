---
'@repo/mcp-common': patch
'docs-ai-search': patch
'workers-bindings': patch
'workers-observability': patch
---

Set `destructiveHint: false` and `openWorldHint: false` on `search_cloudflare_documentation` and `migrate_pages_to_workers_guide`. Both only read Cloudflare's own documentation, but without explicit values clients fall back to the MCP spec defaults (`destructiveHint: true`, `openWorldHint: true`).
