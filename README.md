# Martina MCP connector

[Martina](https://getmartina.com/) is an AI marketing cofounder with nine specialist teammates. This repository contains **public connection metadata and documentation only** for the hosted Martina service. Martina is a proprietary SaaS. Its application, server implementation and private source code are not included or licensed by this repository.

## What Martina does

| Teammate | Marketing work |
| --- | --- |
| Otto | Email outreach |
| Remy | Reddit |
| Lina | LinkedIn |
| Theo | Lead scouting |
| Lana | Launches and directory submissions |
| Simon | SEO, GEO and AEO |
| Sofi | Social media |
| Iris | Brand design |
| Veda | Video |

Your team uses your accounts and a shared Business Brain. Martina provides an activity dashboard and per-teammate Draft or Autopilot settings.

## Requirements

An active Martina plan and an AI client that supports remote MCP are required. Connect the accounts needed for your requested marketing channels. Use OAuth to sign in and choose the product the agent may work on. Never put an API key or OAuth token in a public repository.

## Connect

The hosted Streamable HTTP endpoint is:

```
https://getmartina.com/api/mcp
```

In an MCP client such as Cursor, add a remote server named `martina` with this URL and complete the sign-in flow. This plugin contains only that remote connection configuration. No local runtime or Martina source download is required.

For Claude Code, the public setup guide documents:

```sh
claude mcp add --transport http martina https://getmartina.com/api/mcp --scope user
```

Then authenticate through `/mcp`. Read the [Claude Code setup guide](https://getmartina.com/docs/claude-code) for current instructions and [agent access guide](https://getmartina.com/docs/agent-access) for client differences. Martina’s scheduled workflows require Claude Code or Codex; other compatible MCP clients can request individual tasks.

## Example requests

- Ask Otto, Remy and Lina to prepare outreach drafts for my product using the Business Brain.
- Ask Lana to prepare a launch and directory submission plan for my product.
- Ask Simon to plan SEO, GEO and AEO content, then coordinate supporting creative with Sofi, Iris and Veda.

These are suggested requests based on Martina’s published teammate roles, not transcripts of completed test runs.

## Documentation and support

- [Product website](https://getmartina.com/)
- [Documentation](https://getmartina.com/docs)
- [Current plans and pricing](https://getmartina.com/pricing)
- [Privacy policy](https://getmartina.com/privacy)
- [Service terms](https://getmartina.com/terms)
- Support: hello@trymartina.com
- Official MCP Registry name: `com.getmartina/martina`

## Scope of this repository

The MIT license covers only the connection metadata and documentation authored in this repository. The Martina name and logo remain brand assets; no trademark rights are granted. Access to the hosted SaaS remains governed by Martina’s plan and service terms. This repository contains no API keys, customer data, backend code or application implementation.
