# mcp-server-weather

This repository contains a simple example of an MCP server that provides weather information for a given location in the United States. This example is from: [Model Context Protocol – Build an MCP Server](https://modelcontextprotocol.io/quickstart/server).

## Using the MCP server with Cursor

Add the `"weather"` object to your `.cursor/mcp.json` file:

```json
{
  "mcpServers": {

    "weather": {
      "command": "uv",
      "args": [
        "--directory",
        "absolute/path/to/mcp-server-weather",
        "run",
        "weather.py"
      ]
    }

  }
}
```
