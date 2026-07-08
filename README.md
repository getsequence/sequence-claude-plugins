# sequence-claude-plugins

Official Claude Code plugin marketplace for [Sequence](https://getsequence.io).

## Install

```
/plugin marketplace add getsequence/sequence-claude-plugins
/plugin install sequence@sequence-claude-plugins
```

On first use of a Sequence tool, Claude Code will prompt you to sign in via OAuth — no manual
API key needed.

## What's included

- **`sequence`** — read-only access to your Sequence accounts, transfers, rules, and audit logs
  via the [Sequence MCP server](https://github.com/getsequence/sequence/blob/main/docs/MCP.md).

## What it can access

The plugin only ever gets a `read:mcp` scoped token — there is no write access in v1. That token
maps to:

- Accounts
- Transfers
- Rules and rule executions
- Audit logs

It cannot move money, create/edit rules, or change any account settings.

## Authentication

Sign-in uses OAuth 2.1 (Auth0) — Claude Code opens a browser login on first use, then reuses a
scoped, revocable token for your org. No API key to copy or store. See the
[MCP OAuth docs](https://github.com/getsequence/sequence/blob/main/docs/MCP.md#oauth-21-authentication)
for how the flow works.

## Support

Issues or questions: support@getsequence.io, or open an issue on this repo.

## Development

Test locally before publishing changes:

```
/plugin marketplace add ./sequence-claude-plugins
/plugin install sequence@sequence-claude-plugins
```
