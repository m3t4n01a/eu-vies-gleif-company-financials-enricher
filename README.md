# EU VIES VAT, Corporate Registry & Financials Enricher

[![Run on Apify Store](https://img.shields.io/badge/Apify_Store-Run_Actor-00C853?style=for-the-badge&logo=apify)](https://apify.com/willowy_catamaran_fco/eu-vies-gleif-company-enricher)

Verify European VAT numbers via official VIES API, extract 27-country registry & balance sheet financials (GLEIF + ANAF), and enrich verified B2B emails.

---

## 1-Click n8n Workflow Template (Ready to Import)
Import directly into **n8n** (`Workflows -> Import from URL`) using:
`https://raw.githubusercontent.com/m3t4n01a/eu-vies-gleif-company-financials-enricher/main/n8n-workflow.json`

Or download [`n8n-workflow.json`](./n8n-workflow.json) from this repository.

## Claude Desktop / Cursor MCP Server Integration
Use this B2B intelligence engine directly inside Claude Desktop, Cursor, or Windsurf:
```json
{
  "mcpServers": {
    "eu-vies-gleif-company-enricher": {
      "command": "npx",
      "args": [
        "-y",
        "@apify/actors-mcp-server",
        "--actors",
        "willowy_catamaran_fco/eu-vies-gleif-company-enricher"
      ],
      "env": {
        "APIFY_TOKEN": "YOUR_APIFY_API_TOKEN"
      }
    }
  }
}
```

## Direct Synchronous REST API (cURL / Clay / Make)
```bash
curl -X POST "https://api.apify.com/v2/acts/willowy_catamaran_fco~eu-vies-gleif-company-enricher/run-sync-get-dataset-items?token=YOUR_APIFY_API_TOKEN" \
  -H 'Content-Type: application/json' \
  -d '{"vatCodesOrCompanyNames": ["RO14399840", "Siemens AG"], "defaultCountryCode": ""}'
```