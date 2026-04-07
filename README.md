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

### CLI

- Repo: https://github.com/henu-wang/tokrepo-cli
- npm: https://www.npmjs.com/package/tokrepo

### MCP server

- Repo: https://github.com/henu-wang/tokrepo-mcp-server
- Official MCP Registry: `io.github.henu-wang/tokrepo-mcp-server`
- npm: https://www.npmjs.com/package/tokrepo-mcp-server

### Cross-platform skill

- Repo: https://github.com/henu-wang/tokrepo-search-skill
- Includes Claude Code, Codex, Cursor, Gemini CLI, and `AGENTS.md` variants

## Quick Use

Install the CLI:

```bash
npm install -g tokrepo
```

Search and install:

```bash
tokrepo search "mcp database"
tokrepo install <name-or-uuid>
```

Or use without installing:

```bash
npx tokrepo search "claude code"
npx tokrepo install awesome-cursor-rules
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
- CLI: https://github.com/henu-wang/tokrepo-cli | [npm](https://www.npmjs.com/package/tokrepo)
- MCP server: https://github.com/henu-wang/tokrepo-mcp-server | [npm](https://www.npmjs.com/package/tokrepo-mcp-server)
- MCP Registry listing: `io.github.henu-wang/tokrepo-mcp-server`
- Skill repo: https://github.com/henu-wang/tokrepo-search-skill
