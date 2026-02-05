# Currency MCP

**Real-time currency conversion for AI agents and Claude Code**

[![MCP Compatible](https://img.shields.io/badge/MCP-Compatible-blue)](https://modelcontextprotocol.io)
[![Currencies](https://img.shields.io/badge/Currencies-9-green)](https://currency-mcp.com)

Give your AI assistant the power to convert currencies with live exchange rates. Currency MCP provides a simple, reliable Model Context Protocol server for currency operations.

## Features

- **Real-time rates** — Live exchange rates from reliable financial data sources
- **9 major currencies** — USD, EUR, GBP, JPY, CHF, CAD, AUD, CNY, INR
- **Smart caching** — 1-hour rate caching for fast, efficient responses
- **Simple API** — Three tools: convert, get rate, list currencies
- **Zero config** — Just add the MCP server URL and start converting

## Quick Start

Add the Currency MCP server to your Claude Code configuration:

```json
{
  "mcpServers": {
    "currency": {
      "type": "url",
      "url": "https://currency-mcp.com/sse"
    }
  }
}
```

Then ask Claude:
- "Convert 500 EUR to USD"
- "What's the current GBP to JPY rate?"
- "List available currencies"

## Supported Currencies

| Code | Currency | Code | Currency |
|------|----------|------|----------|
| USD | US Dollar | CAD | Canadian Dollar |
| EUR | Euro | AUD | Australian Dollar |
| GBP | British Pound | CNY | Chinese Yuan |
| JPY | Japanese Yen | INR | Indian Rupee |
| CHF | Swiss Franc | | |

## Tools

| Tool | Description |
|------|-------------|
| `convert_currency` | Convert an amount between currencies |
| `get_rate` | Get the exchange rate between two currencies |
| `list_currencies` | List all supported currencies |

## Learn More

Visit [currency-mcp.com](https://currency-mcp.com) for documentation and updates.

---

Built for the [Model Context Protocol](https://modelcontextprotocol.io) ecosystem.
