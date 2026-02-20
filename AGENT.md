# AGENT.md — Nexmo Conversion API CLI for AI Agents

This document explains how to use the Nexmo Conversion API CLI as an AI agent.

## Overview

The `nexmo` CLI provides SMS and communication conversion tracking via the Nexmo Conversion API API.

## Prerequisites

```bash
nexmo config set --api-key <key>
```

## All Commands

### Config

```bash
nexmo config set --api-key <key>
nexmo config set --base-url <url>
nexmo config show
```

### Items

```bash
nexmo list                      # List all items
nexmo list --json               # JSON output
nexmo get <id>                  # Get item details
nexmo get <id> --json           # JSON output
```

## Tips for Agents

1. Always use `--json` when parsing results programmatically
2. Use `nexmo list --json` to get all items as structured data
3. Use `nexmo get <id> --json` for detailed item information
4. All commands return structured data suitable for automation
