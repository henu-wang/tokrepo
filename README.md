# TokRepo

TokRepo is an open registry for AI assets.

It helps humans and agents find, inspect, and install:

- skills
- prompts
- MCP configs
- scripts
- workflows

Website: https://tokrepo.com

## GitHub Entry Points

### MCP server

- Repo: https://github.com/henu-wang/tokrepo-mcp-server
- Official MCP Registry: `io.github.henu-wang/tokrepo-mcp-server`
- npm: https://www.npmjs.com/package/tokrepo-mcp-server

### Cross-platform skill

- Repo: https://github.com/henu-wang/tokrepo-search-skill
- Includes Claude Code, Codex, Cursor, Gemini CLI, and `AGENTS.md` variants

## Quick Use

Search TokRepo:

```bash
npx tokrepo search "mcp database"
npx tokrepo search "claude code"
```

Install from TokRepo:

```bash
npx tokrepo install <uuid-or-name>
```

Add TokRepo as an MCP server:

```bash
claude mcp add tokrepo -- npx tokrepo-mcp-server
codex --mcp-server tokrepo -- npx tokrepo-mcp-server
gemini settings mcp add tokrepo -- npx tokrepo-mcp-server
```

## Why This Repo Exists

Most GitHub discovery still happens through repository names, README text, topics, and linked repos.

This repo is the canonical GitHub landing page for TokRepo so that:

- developers can understand the product quickly
- AI agents can find the right MCP and skill repos
- awesome-list maintainers have a stable GitHub reference

## Links

- Website: https://tokrepo.com
- CLI: https://www.npmjs.com/package/tokrepo
- MCP package: https://www.npmjs.com/package/tokrepo-mcp-server
- MCP Registry listing: `io.github.henu-wang/tokrepo-mcp-server`
- MCP repo: https://github.com/henu-wang/tokrepo-mcp-server
- Skill repo: https://github.com/henu-wang/tokrepo-search-skill
