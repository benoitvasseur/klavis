<div align="center">
  <picture>
    <img src="https://raw.githubusercontent.com/klavis-ai/klavis/main/static/klavis-ai.png" width="80">
  </picture>
</div>

<h1 align="center">Production-ready MCP integrations for AI applications</h1>

[![Documentation](https://img.shields.io/badge/Documentation-📖-green)](https://docs.klavis.ai)
[![Website](https://img.shields.io/badge/Website-🌐-purple)](https://www.klavis.ai)
[![Discord](https://img.shields.io/badge/Discord-Join-7289DA?logo=discord&logoColor=white)](https://discord.gg/p7TuTEcssn)
[![YouTube Demo](https://img.shields.io/badge/Demo-YouTube-red)](https://www.youtube.com/@KlavisAI-w2l)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

## Introduction

Klavis AI makes it effortless to connect to production-ready MCP servers & clients at scale. Integrate MCPs with your AI applications in a minute, and scale to millions of users using our open-source infrastructure, hosted servers, and multi-platform clients!

## ✨ Key Features

Klavis AI removes the barrier to using MCPs by providing:

- **Production-Ready MCP Servers**: All our MCP Servers come from official sources or are internally evaluated by Klavis and our customers.
- **Built-In Authentications**: Secure authentication out of the box for both developers and end-users.
- **MCP Client Integrations**: We support MCP Client Integration, allowing you to interact via Klavis Slack, Discord, or web MCP client and integrate into your workflows seamlessly.
- **100+ Tool Integrations & Customizations**: Support for various tools and customized MCP servers tailored to your needs.

## 🚀 Quick Start

To run self hosted versions, check out the detailed readme in each MCP server and MCP client below.

### MCP Servers

- [**Discord**](mcp_servers/discord/README.md): For Discord API integration
- [**Document Conversion (Pandoc)**](mcp_servers/pandoc/README.md): Convert between various file formats using Pandoc
- [**Firecrawl**](mcp_servers/firecrawl/README.md): For web crawling and data collection
- [**Firecrawl Deep Research**](mcp_servers/firecrawl_deep_research/README.md): For deeper web research tasks
- [**GitHub**](mcp_servers/github/README.md): Perform GitHub repository operations
- [**Markitdown**](mcp_servers/markitdown/README.md): Markdown conversion tool
- [**Postgres**](mcp_servers/postgres/README.md): For PostgreSQL database operations
- [**Report Generation**](mcp_servers/report_generation/README.md): Create professional web reports from user query
- [**Resend**](mcp_servers/resend/README.md): For email services
- [**Shopify**](mcp_servers/shopify/README.md): For Shopify Admin API integration
- [**Slack**](mcp_servers/slack/README.md): For Slack API integration
- [**Supabase**](mcp_servers/supabase/README.md): For database operations
- [**YouTube**](mcp_servers/youtube/README.md): Extract and convert YouTube video information
- [**Jira**](mcp_servers/jira/README.md): manage your sprint
- And More!

### MCP Clients

- [**Discord MCP Client Setup Guide**](mcp-clients/README-Discord.md)
- [**Slack MCP Client Setup Guide**](mcp-clients/README-Slack.md)
- [**Web Chat MCP Client Setup Guide**](mcp-clients/README-Web.md)

### Hosted solutions

1. **Sign up for Klavis platform and create your [API key](https://www.klavis.ai/home/api-keys)**

2. **Create a new MCP server instance**

```bash
curl --request POST \
  --url https://api.klavis.ai/mcp-server/instance/create \
  --header 'Authorization: Bearer <KLAVIS_API_KEY>' \
  --header 'Content-Type: application/json' \
  --data '{
  "serverName": "<MCP_SERVER_NAME>",
  "userId": "<USER_ID>",
  "platformName": "<PLATFORM_NAME>"
}'
```

> **Note:** It will return an MCP server URL that takes care of everything for you!

3. **Set up auth token or use our in-house OAuth flow (if the MCP Server requests private info)**

```bash
curl --request POST \
  --url https://api.klavis.ai/mcp-server/instance/set-auth-token \
  --header 'Authorization: Bearer <KLAVIS_API_KEY>' \
  --header 'Content-Type: application/json' \
  --data '{
  "instanceId": "<string>",
  "authToken": "<string>"
}'
```

Check out our [documentation](https://docs.klavis.ai) for more details!

## 🤝 Contributing

We love contributions! Please check our [Contributing Guidelines](CONTRIBUTING.md) for details on how to submit changes. Join our [Discord community](https://discord.gg/p7TuTEcssn) to discuss ideas and get help.

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
