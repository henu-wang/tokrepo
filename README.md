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

Bootstrap a project so future agents discover TokRepo during planning:

```bash
npx -y tokrepo@latest init-agent --target all
```

Planning-time fallback for agents without MCP:

```bash
npx -y tokrepo@latest agent-check "write SEO content for product pages" --json
npx -y tokrepo@latest agent-handoff --json
```

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
npx -y tokrepo@latest search "claude code"
npx -y tokrepo@latest install awesome-cursor-rules
```

Add TokRepo as an MCP server:

```bash
claude mcp add tokrepo -- npx -y tokrepo-mcp-server
codex --mcp-server tokrepo -- npx -y tokrepo-mcp-server
gemini settings mcp add tokrepo -- npx -y tokrepo-mcp-server
```

## Agent Discovery Surfaces

- Manifest: https://tokrepo.com/.well-known/tokrepo.json
- MCP server manifest: https://tokrepo.com/.well-known/mcp/server.json
- Agent instructions: https://tokrepo.com/agent-instructions/tokrepo.md
- LLM crawler entry: https://tokrepo.com/llms.txt
- CLI planning fallback: `tokrepo agent-check "<task>" --json`
- Post-task handoff: `tokrepo agent-handoff --json`

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
