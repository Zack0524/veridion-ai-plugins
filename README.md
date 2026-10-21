# Veridion Markets for AI tools

Receipt-linked U.S. congressional (House and Senate), executive-branch (OGE) and SEC Form 4 disclosures, for your AI tools. Every row links to the government document it came from. The server is read-only and needs no key.

MCP server: `https://www.veridionmarkets.com/api/mcp` (streamable HTTP)

## Cursor

Install this plugin from the Cursor Marketplace, or add the server directly in `.cursor/mcp.json`:

```json
{ "mcpServers": { "veridion": { "url": "https://www.veridionmarkets.com/api/mcp" } } }
```

## Gemini CLI

```bash
gemini extensions install https://github.com/Zack0524/veridion-ai-plugins
```

## Tools

- `search_disclosures`: receipt-linked rows and point-in-time history.
- `get_disclosure_history`: every observed version of one filing.
- `list_members`: resolves filers.
- `get_coverage`: measured counts.
- `get_status`: source state.

The server's `tools/list` response is the authority on what it exposes.

## Example prompts

- Show the five most recent House stock disclosures, with the filing receipt for each.
- What did [member name] disclose in the last 90 days? Include the government document for every transaction.
- What is the current status of each Veridion source?

An empty answer means no served rows matched. It is not proof that no filing exists.

Docs: https://www.veridionmarkets.com/data-api · Terms: https://www.veridionmarkets.com/data-api/license
