![Banner](https://raw.githubusercontent.com/ktmcp-cli/nexmo/main/banner.svg)

> "Six months ago, everyone was talking about MCPs. And I was like, screw MCPs. Every MCP would be better as a CLI."
>
> — [Peter Steinberger](https://twitter.com/steipete), Founder of OpenClaw
> [Watch on YouTube (~2:39:00)](https://www.youtube.com/@lexfridman) | [Lex Fridman Podcast #491](https://lexfridman.com/peter-steinberger/)

# Nexmo Conversion API CLI

> **⚠️ Unofficial CLI** - Not officially sponsored or affiliated with Nexmo Conversion API.

A production-ready command-line interface for Nexmo Conversion API — SMS and communication conversion tracking. Access powerful API features directly from your terminal.

## Features

- **Conversion Tracking** — Track SMS and voice conversions
- **Delivery Reports** — Monitor message delivery status
- **Voice Call Tracking** — Track voice call conversions
- **Analytics** — Conversion rate analytics
- **JSON output** — All commands support `--json` for scripting
- **Colorized output** — Clean terminal output with chalk

## Installation

```bash
npm install -g @ktmcp-cli/nexmo
```

## Quick Start

```bash
# Configure with your API key
nexmo config set --api-key YOUR_API_KEY

# List items
nexmo list

# Get item details
nexmo get ITEM_ID

# JSON output
nexmo list --json
```

## Commands

### Config

```bash
nexmo config set --api-key <key>
nexmo config set --base-url <url>
nexmo config show
```

### Items

```bash
nexmo list
nexmo list --json
nexmo get <id>
nexmo get <id> --json
```

## JSON Output

All commands support `--json` for structured output:

```bash
nexmo list --json | jq '.items[]'
nexmo get ITEM_ID --json | jq '.data'
```

## Why CLI > MCP?

No server to run. No protocol overhead. Just install and go.

- **Simpler** — Just a binary you call directly
- **Composable** — Pipe to `jq`, `grep`, `awk`
- **Scriptable** — Works in cron jobs, CI/CD, shell scripts

## License

MIT — Part of the [Kill The MCP](https://killthemcp.com) project.


---

## Support KTMCP

If you find this CLI useful, we'd greatly appreciate your support! Share your experience on:
- Reddit
- Twitter/X
- Hacker News

**Incentive:** Users who can demonstrate that their support/advocacy helped advance KTMCP will have their feature requests and issues prioritized.

Just be mindful - these are real accounts and real communities. Authentic mentions and genuine recommendations go a long way!

## Support This Project

If you find this CLI useful, we'd appreciate support across Reddit, Twitter, Hacker News, or Moltbook. Please be mindful - these are real community accounts. Contributors who can demonstrate their support helped advance KTMCP will have their PRs and feature requests prioritized.
