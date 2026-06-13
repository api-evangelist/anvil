# Anvil

Anvil is a PDF infrastructure platform providing REST and GraphQL APIs for filling PDF templates with JSON data, generating PDFs from HTML or Markdown, collecting e-signatures (Etch), building web forms, and extracting data from documents via OCR and Document AI. It is designed for developers embedding paperwork automation into applications across HR, insurance, financial services, and legal workflows.

- **Website:** https://www.useanvil.com/
- **Developer Docs:** https://www.useanvil.com/docs/
- **GitHub Org:** https://github.com/anvilco
- **Pricing:** https://www.useanvil.com/pricing/
- **Status:** https://status.useanvil.com/
- **Blog:** https://www.useanvil.com/blog/
- **LinkedIn:** https://www.linkedin.com/company/anvil-foundry
- **X:** https://x.com/useanvil

## APIs

| API | Type | Description |
|-----|------|-------------|
| PDF Filling API | REST | Fill existing PDF templates with JSON data |
| PDF Generation API | REST | Generate PDFs from HTML, CSS, or Markdown |
| Etch E-Sign API | GraphQL | Embed white-labeled e-signature collection |
| GraphQL API | GraphQL | Primary interface for all Anvil operations |
| Document AI & OCR API | GraphQL | Extract structured data from uploaded documents |
| Webhooks | Events | Receive HTTP callbacks for workflow events |

## Authentication

API keys using HTTP Basic Auth. Two key types: development (watermarked, 4 req/sec) and production (plan-based limits). Keys are server-side only — not for browser use.

## SDKs

- Node.js: https://github.com/anvilco/node-anvil
- Python: https://github.com/anvilco/python-anvil
- C#/.NET: https://github.com/anvilco/dotnet-anvil
- React UI: https://github.com/anvilco/react-ui

## Pricing Summary

| Plan | Monthly | Annual | Rate Limit |
|------|---------|--------|------------|
| Free | $0 | $0 | 4 req/sec |
| AI Pack | $99 | $79/mo | 4 req/sec |
| Product Pack | $425 | $340/mo | 40 req/sec |
| Enterprise | Custom | Custom | Custom |

Overages: $0.10/PDF, $1.00/workflow submission, $1.50/e-sign packet.

## Repository Structure

```
apis.yml                          # APIs.json 0.19 index
plans/anvil-plans-pricing.yml     # API Commons Plans 0.1
rate-limits/anvil-rate-limits.yml # API Commons Rate Limits 0.1
finops/anvil-finops.yml           # FinOps Framework 1.0 FOCUS-aligned
```
