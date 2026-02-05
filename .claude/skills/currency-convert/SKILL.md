# Currency Conversion Skill

Convert currencies using real-time exchange rates via the Currency MCP server.

## MCP Server Configuration

This skill requires connecting to the remote Currency MCP server. Add this to your MCP settings:

```json
{
  "mcpServers": {
    "currency": {
      "type": "url",
      "url": "https://currency-mcp.com/mcp"
    }
  }
}
```

## Available Tools

### `convert_currency`
Convert an amount from one currency to another.

**Parameters:**
- `amount` (number): The amount to convert
- `from` (string): Source currency code (e.g., "USD")
- `to` (string): Target currency code (e.g., "EUR")

### `get_rate`
Get the current exchange rate between two currencies.

**Parameters:**
- `from` (string): Source currency code
- `to` (string): Target currency code

### `list_currencies`
List all supported currencies with their names.

**Parameters:** None

## Supported Currencies

| Code | Currency |
|------|----------|
| USD | US Dollar |
| EUR | Euro |
| GBP | British Pound |
| JPY | Japanese Yen |
| CHF | Swiss Franc |
| CAD | Canadian Dollar |
| AUD | Australian Dollar |
| CNY | Chinese Yuan |
| INR | Indian Rupee |

## Usage Examples

**Convert 100 USD to EUR:**
"Convert 100 dollars to euros"

**Get current exchange rate:**
"What's the exchange rate from GBP to JPY?"

**List available currencies:**
"What currencies are supported?"

## Notes

- Exchange rates are cached for 1 hour for performance
- Rates are sourced from reliable financial data providers
- All conversions use mid-market rates
