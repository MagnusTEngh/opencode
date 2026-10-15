# OpenCode Config

Keep this repository's OpenCode setup simple, portable, and secure.

## Before proceeding

1. Read the README.md file.

## Security

* Never commit API keys, tokens, passwords, or other secrets.
* Never print, log, read, or expose secret environment variables.
* Reference secrets only through environment variables such as `{env:OPENAI_API_KEY}`.
* Keep `.env` and other secret files out of Git.
* Do not add external services, plugins, or MCP servers without explicit user approval.

## MCP

* Prefer self-hosted MCP servers.
* Keep credentials in environment variables, never in `opencode.jsonc`.
* Give MCP servers the minimum access they need.
* Require user approval for MCP tools that can modify files, execute commands, access credentials, or perform external actions.
* Prefer authenticated HTTPS for remote MCP servers; do not expose unauthenticated MCP endpoints publicly.

## Changes

Prefer small, auditable configuration changes. When security and convenience conflict, choose the safer configuration and explain the tradeoff.
