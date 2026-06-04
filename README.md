# Washington University in St. Louis (washington-university-in-st-louis)

Washington University in St. Louis (WashU) is a private research university in St. Louis, Missouri, ranked #171 in the QS World University Rankings 2025. This repository catalogs WashU's public developer and API footprint as an [APIs.json](https://apisjson.org) provider profile for the API Evangelist network.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/washington-university-in-st-louis/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=washington-university-in-st-louis-api-evangelist&utm_content=repo

## Type

- Index / Consumer / 3rd-Party

## Tags

Education, Higher Education, University, Research, United States, MuleSoft, OAI-PMH

## APIs

- **WashU Enterprise Integration APIs (MuleSoft Anypoint)** — Institutional integration APIs (Person, Financial, Supplier, Location, Academic, Organization) published via MuleSoft Anypoint Exchange. Access is gated through ServiceNow for WashU integrators.
  - Docs: https://data.wustl.edu/api-portal/
  - How-to: https://data.wustl.edu/api-portal/api-portal-how-to-documents/
  - Access: https://data.wustl.edu/api-portal/api-portal-anypoint-access/
  - Anypoint Exchange: https://anypoint.mulesoft.com/exchange/portals/wustl/
- **Digital Commons Data@Becker (Research Repository)** — School of Medicine / Becker Medical Library research data repository on the Elsevier Digital Commons Data (Mendeley Data) platform with a live OAI-PMH endpoint.
  - Docs: https://digitalcommonsdata.wustl.edu/api/docs/
  - OAI-PMH: https://digitalcommonsdata.wustl.edu/oai?verb=Identify

## Plans / Rate Limits / FinOps

- Plans & Pricing: [plans/washington-university-in-st-louis-plans-pricing.yml](plans/washington-university-in-st-louis-plans-pricing.yml)
- Rate Limits: [rate-limits/washington-university-in-st-louis-rate-limits.yml](rate-limits/washington-university-in-st-louis-rate-limits.yml)
- FinOps: [finops/washington-university-in-st-louis-finops.yml](finops/washington-university-in-st-louis-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-06-03

## Common Properties

- Website: https://wustl.edu
- GitHub: https://github.com/wustl
- LinkedIn: https://www.linkedin.com/school/washington-university-in-st-louis/
- Developer Portal: https://data.wustl.edu/api-portal/
- Review: [review.yml](review.yml)

## Notes

All URLs in this profile were probed and resolved (HTTP 200) on 2026-06-03, except the LinkedIn school page which returns 999 due to LinkedIn anti-bot protection (the page exists). The WashU MuleSoft Anypoint APIs are real but **gated** — access requires a ServiceNow request and is limited to WashU integrators, not open public consumption. No public open-data portal or documented course/SIS API was confirmed. No endpoints were fabricated.

## Maintainers

- Kin Lane — kin@apievangelist.com
