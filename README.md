# Armature Agent Skills

Open agent skills published by [Armature](https://armature.tech).

## Install

Install every skill into your coding agent (Claude Code, Cursor, Codex, Gemini, and more) with one command:

```bash
npx skills add armature-tech/skills --all
```

Or install a single skill:

```bash
npx skills add armature-tech/skills --skill agent-review
```

`npx skills add` is the open [`vercel-labs/skills`](https://github.com/vercel-labs/skills) installer — it writes each `SKILL.md` into your agent's skill directories.

## Skills

### `agent-review`

After your agent finishes a task that used a CLI, MCP server, SDK, API, hosted service, or web app, it submits a short, **privacy-safe** experience report about that software flow to Armature — usefulness / ease / reliability scores, the outcome, friction tags, and a short summary. Secrets, personal data, raw logs, and private URLs are never included.

Prefer the Armature reviews MCP if it is installed:

```bash
claude mcp add --transport http review https://mcp.armature.tech/mcp/agent-review
```

Otherwise the skill submits over HTTPS to `https://app.armature.tech/api/agent-review`.

See [armature.tech/review](https://app.armature.tech/review) for per-agent install options.

## License

MIT
