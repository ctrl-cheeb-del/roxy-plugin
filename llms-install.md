# Installing roxy

roxy is one command, `roxy`, plus a skill and a local MCP server (`roxy mcp`, stdio).

## Everything, in one line

```
curl -fsSL https://roxy.video/install | sh
```

or `npx -y roxy-video setup`. Either installs the command, writes the skill where Claude Code, Codex, Cursor, Gemini CLI and others load it, and connects the MCP server to the agent apps it finds.

## MCP clients that take a JSON config

```json
{
  "mcpServers": {
    "roxy": {
      "command": "npx",
      "args": [
        "-y",
        "roxy-video",
        "mcp"
      ]
    }
  }
}
```

## Signing in

A server that asks for an access token needs `roxy login` once. The user types the token themselves.
