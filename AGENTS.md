# roxy agent plugin

Generated from the roxy repository (`plugin/build.ts`): do not edit here.

The repository root is the plugin. Every host reads the same `skills/` folder and starts the same MCP server (`npx -y roxy-video mcp`).

| Host | Manifest | MCP config |
|---|---|---|
| Claude Code | `.claude-plugin/plugin.json`, marketplace `.claude-plugin/marketplace.json` | `.mcp.json` |
| Cursor | `.cursor-plugin/plugin.json` | `.mcp.json` |
| OpenAI Codex | `.codex-plugin/plugin.json`, marketplace `.agents/plugins/marketplace.json` | `.mcp.json` |
| Gemini CLI | `gemini-extension.json`, context `GEMINI.md` | inline |
| Google Antigravity | `.antigravity-plugin/plugin.json` | `mcp_config.json` |
| Grok Build | `.grok-plugin/plugin.json` | `.mcp.json` |
| skills.sh and other Agent Skills hosts | `skills/roxy/SKILL.md` | none: the skill says how to install the command |

There is one skill on purpose. Measured with fresh agents and plain requests, one skill was reached for every time; the same skill beside eight more split by job was reached for less than half the time.
