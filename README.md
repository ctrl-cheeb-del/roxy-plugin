# roxy

**A machine your agent edits video on.** https://roxy.video

Claude Code, Codex and Cursor already know how to edit: they write the cut as commands. roxy is where those commands run: a box with ffmpeg, Remotion, Python and headless Chrome on it, your footage one command away, a page to review the cut on, and a link for whatever comes out. roxy does not edit for you. It is the room, the machine and the tools.

## Install

```
curl -fsSL https://roxy.video/install | sh
```

That installs the `roxy` command, the skill, and the MCP tools in every agent app it finds. Then ask your agent for anything to do with a video:

> Edit the video in ./footage into a first cut.

> Make three TikToks out of this podcast episode.

> Add word-by-word captions to demo.mov and send me a link.

### Other ways in

| | |
|---|---|
| npm | `npx -y roxy-video setup` |
| Skill only, any agent | `npx skills add ctrl-cheeb-del/roxy-plugin` or `npx skills add https://roxy.video` |
| Claude Code plugin | `/plugin marketplace add ctrl-cheeb-del/roxy-plugin` then `/plugin install roxy@roxy` |
| Claude Code, tools only | `claude mcp add --scope user roxy -- npx -y roxy-video mcp` |
| Codex, tools only | `codex mcp add roxy -- npx -y roxy-video mcp` |
| Gemini CLI | `gemini extensions install https://github.com/ctrl-cheeb-del/roxy-plugin` |
| Any MCP client | see [llms-install.md](llms-install.md) |

## What your agent gets

- `roxy new`, `put`, `push`: a box, with your footage or project in it, in seconds
- `roxy exec`: any command, on a machine with many CPUs
- `roxy hear`, `look`: what is said and when, and frames, so it can check its own cut
- `roxy review`, `notes`: a link where you watch the cut and pin notes to moments, which come back to the agent
- `roxy export`: the file fitted to TikTok, Instagram, Shorts, YouTube or 4K

The whole guide is in [the skill](skills/roxy/SKILL.md).

## License

MIT
