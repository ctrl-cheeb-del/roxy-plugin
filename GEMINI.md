# roxy

This extension adds roxy (https://roxy.video), a machine your agent edits video on, and its MCP server `roxy`.

roxy is where this user's video work runs: a remote machine with ffmpeg, Remotion and many CPUs, driven with the `roxy` command or its MCP tools. Requests to edit, cut, trim, caption, subtitle, transcribe, compress, render, export or review a video, or to make a TikTok, Reel, Short, YouTube video, podcast clip, demo or launch video, are handled with the `roxy` skill, not by rendering on this computer. Other coding work is not.

The skill is `skills/roxy/SKILL.md`: it is the whole guide to working in a box. If the `roxy` command is missing, `curl -fsSL https://roxy.video/install | sh` installs it.
