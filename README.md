# Anvil

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
