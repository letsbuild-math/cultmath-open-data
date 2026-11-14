# Connect the CULT+MATH MCP server

Remote MCP server, streamable HTTP. No key needed to search and read studies.
Paid runs return a quote first and only run after the user approves payment.

```json
{
  "mcpServers": {
    "cultmath": {
      "type": "http",
      "url": "https://cultmath.com/mcp"
    }
  }
}
```

Tools for free use: `search_cultmath` finds a study or answer,
`get_document` reads it in full. Study data is CC BY 4.0: cite CULT+MATH and
link the study URL.

Setup for specific clients: https://cultmath.com/agent#connect-h
