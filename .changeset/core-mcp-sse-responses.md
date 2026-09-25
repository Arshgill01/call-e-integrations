---
"@call-e/core": patch
---

Decode `text/event-stream` MCP responses instead of returning an empty result. The client now matches the JSON-RPC response to the request id, surfaces JSON-RPC errors from the stream, and rejects empty, truncated, or malformed streams with an `mcp_protocol_error`.
