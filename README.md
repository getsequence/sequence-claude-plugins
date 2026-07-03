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

## Development

Test locally before publishing changes:

```
/plugin marketplace add ./sequence-claude-plugins
/plugin install sequence@sequence-claude-plugins
```
