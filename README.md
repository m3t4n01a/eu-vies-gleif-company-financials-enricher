# EU VIES VAT, Corporate Registry & Financials Enricher

[![Run on Apify Store](https://img.shields.io/badge/Apify_Store-Run_Actor-00C853?style=for-the-badge&logo=apify)](https://apify.com/willowy_catamaran_fco/eu-vies-gleif-company-enricher)

Verify European VAT numbers via official VIES API, extract 27-country registry & balance sheet financials (GLEIF + ANAF), and enrich verified B2B emails.

## 1-Click Synchronous API Execution (n8n / Clay / Claude MCP)
```bash
curl -X POST "https://api.apify.com/v2/acts/willowy_catamaran_fco~eu-vies-gleif-company-enricher/run-sync-get-dataset-items?token=YOUR_APIFY_TOKEN" \
  -H "Content-Type: application/json" -d '{}'
```