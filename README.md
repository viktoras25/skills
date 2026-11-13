# viktoras25 marketplace

A [Claude Code plugin marketplace](https://code.claude.com/docs/en/plugin-marketplaces) that links my skills and MCP servers. Each plugin lives in its own repository; this repo only lists them.

| Plugin | What it does | Repository |
|---|---|---|
| `video-summary` | Summarize a video from its URL using its subtitles | [video-summary-skill](https://github.com/viktoras25/video-summary-skill) |
| `language-tutor` | Language tutor: placement, lessons, grading, pacing | [language-tutor-skill](https://github.com/viktoras25/language-tutor-skill) |
| `language-memory` | Long-term memory MCP server for the tutor | [language-tutor-mcp](https://github.com/viktoras25/language-tutor-mcp) |

## Install

```
/plugin marketplace add viktoras25/agent-marketplace
/plugin install video-summary@viktoras25
/plugin install language-tutor@viktoras25
/plugin install language-memory@viktoras25
```

`language-memory` connects to a server you deploy yourself (see its README) and asks for your connector URL on install. The URL contains your token, so it is stored in your system's secure credential store, not in settings.

Update with `/plugin marketplace update viktoras25`.

Not using Claude Code? The skills are plain `SKILL.md` folders; copy them from their repositories into your agent's skills directory.
