# Washington University in St. Louis (washington-university-in-st-louis)

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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Washington University in St. Louis (WashU) is a private research university in St. Louis, Missouri. This repository catalogs WashU's public developer and API footprint as an [APIs.json](https://apisjson.org) provider profile for the API Evangelist network, profiled under the **university pipeline** — which settles *who operates* each surface before recording it, because a university is a federation of buyers and most of what appears under its name is a vendor's contract.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/washington-university-in-st-louis/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=washington-university-in-st-louis-api-evangelist&utm_content=repo

## Type

- Index / Provider / 1st-Party — `x-type: university`, `x-category: Private Research University`

## Tags

University, Higher Education, Education, United States, Missouri, Private Research University, Research Data, Research Repository, Identity Federation, Genomics, Bioinformatics, GraphQL, OAI-PMH, Shibboleth, DataCite, MuleSoft

## Surfaces, by who operates them

Every entry carries an `x-operator`. It answers a different question than `method:` does: `method:` says how *we* came to hold an artifact, `x-operator` says **who runs the thing the artifact describes**.

### `institution` — Washington University's own

- **CIViC — Clinical Interpretation of Variants in Cancer** — the one genuinely public, WashU-engineered API. A GraphQL knowledgebase of the clinical significance of cancer variants, built and operated by The McDonnell Genome Institute at WashU School of Medicine and released CC0. 502 types, 112 root queries, 47 mutations; anonymous reads, optional free bearer-token key, 3 req/sec documented.
  - Endpoint: https://civicdb.org/api/graphql · Explorer: https://civicdb.org/api/graphiql
  - Docs: https://docs.civicdb.org/en/latest/api.html · Source: https://github.com/griffithlab/civic-v2
  - Schema: [graphql/washington-university-in-st-louis-civic-schema.graphql](graphql/washington-university-in-st-louis-civic-schema.graphql) — printed from live introspection, `method: probed`
- **WashU Enterprise Integration APIs (MuleSoft Anypoint)** — Person, Financial, Supplier, Location, Academic, Organization. WashU's engineering, MuleSoft's delivery, and entirely closed: access by ServiceNow request, no public spec, endpoint or sign-up.
  - https://data.wustl.edu/api-portal/ · https://data.wustl.edu/api-portal/api-portal-anypoint-access/
- **CNDA (XNAT)** and **BALSA** — real WashU research-data platforms, both auth-walled. CNDA returns its login page under HTTP 200 even at `/xapi/swagger.json`, which is a soft-200 gate, so no contract was taken from either.

### `federation` — shared by definition, and theirs

- **WashU Shibboleth Identity Provider** — entityID `https://login.wustl.edu/idp/shibboleth`, published as signed SAML 2.0 metadata in InCommon with REFEDS Research & Scholarship and SIRTFI assurance, scoped to `wustl.edu`. The strongest institution-operated machine-readable surface WashU has.
  - https://mdq.incommon.org/entities/https%3A%2F%2Flogin.wustl.edu%2Fidp%2Fshibboleth

### `tenant` — WashU's data, someone else's contract

- **WashU Scholarly Repository** — OAI-PMH 2.0, nine metadata formats. `openscholarship.wustl.edu` CNAMEs to `dcwustlmain.bepress.com`; Identify gives `dc-support@elsevier.com`. bepress Digital Commons (Elsevier).
- **Digital Commons Data@Becker** — OAI-PMH 2.0, datacite/oai_dc/oai_datacite. `digitalcommonsdata.wustl.edu` CNAMEs to `www.data.mendeley.com`. Elsevier Digital Commons Data (Mendeley Data).
- **WashU WordPress REST APIs** — every departmental site serves a live, unauthenticated WP REST API with a full route document (data.wustl.edu 467 routes, source.washu.edu 429, washu.edu 337). `data.wustl.edu` CNAMEs to CampusPress; the contract is WordPress core's and the hosting is a vendor's. The content and editorial are WashU's, and in practice this is the only way to read WashU's public content programmatically.

Both were recorded as institution-owned in the June 2026 profile on the strength of a `wustl.edu` label. DNS resolution corrected that. The relationships were kept; only the attribution changed.

### `registry` — memberships, which are facts about them

- **DataCite** — direct member, symbol `WUSTL`, since 2018-08-30, with two registered DOI repositories (`wustl.lib`, `wustl.becker-ir`).
- **ROR** — https://ror.org/01yc7t268 (Funder ID 100007268, GRID grid.4367.6, ISNI 0000 0004 1936 9350).

## Domain standard conformance (education regime)

Conformant, with live evidence: **saml**, **shibboleth**, **oai-pmh** (two endpoints), **datacite**. Explicitly not found, with reasons recorded: crossref, orcid, scim, lti, oneroster, ed-fi, caliper, qti.

- [conformance/washington-university-in-st-louis-conformance.yml](conformance/washington-university-in-st-louis-conformance.yml)

## Artifacts

- GraphQL: [graphql/](graphql/) — CIViC schema + overview
- Authentication: [authentication/washington-university-in-st-louis-authentication.yml](authentication/washington-university-in-st-louis-authentication.yml)
- Conformance: [conformance/washington-university-in-st-louis-conformance.yml](conformance/washington-university-in-st-louis-conformance.yml)
- Plans & Pricing: [plans/washington-university-in-st-louis-plans-pricing.yml](plans/washington-university-in-st-louis-plans-pricing.yml)
- Rate Limits: [rate-limits/washington-university-in-st-louis-rate-limits.yml](rate-limits/washington-university-in-st-louis-rate-limits.yml)
- FinOps: [finops/washington-university-in-st-louis-finops.yml](finops/washington-university-in-st-louis-finops.yml)
- JSON-LD: [json-ld/washington-university-in-st-louis-context.jsonld](json-ld/washington-university-in-st-louis-context.jsonld)
- Domain Security: [security/washington-university-in-st-louis-domain-security.yml](security/washington-university-in-st-louis-domain-security.yml)
- Review: [review.yml](review.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-09-01

## Common Properties

- Website: https://washu.edu (https://wustl.edu 301s here — the institution now presents as WashU)
- GitHub Organization: https://github.com/WashU-IT-RIS · GitHub: https://github.com/wustl
- LinkedIn: https://www.linkedin.com/school/washington-university-in-st-louis/
- Developer Portal: https://data.wustl.edu/api-portal/
- Research Computing: https://ris.wustl.edu/ (user docs at docs.ris.wustl.edu, a meta-refresh into washu.atlassian.net — deliberately not emitted as a `Documentation` pointer, because the audit would then read `atlassian.net` as a domain WashU owns)
- AI Policy / AI Tooling: https://ai.washu.edu/ · https://ai.washu.edu/tools/
- Course Catalog: https://registrar.washu.edu/
- Blog: https://source.washu.edu/

## Notes

All URLs were re-probed on 2026-09-01. Three of them are not plain 200s and are recorded as findings rather than quietly dropped:

- `https://library.washu.edu/` and `https://catalog.wustl.edu/` return **403** behind a Cloudflare bot challenge. That is a fact about their edge, not about their publishing — live, not dead.
- `https://courses.wustl.edu/` now **fails to connect entirely**. It returned 200 in the 2026-06-03 pass. No course or SIS API existed there in either case.
- `https://www.linkedin.com/school/...` returns **999**, LinkedIn's anti-bot code. The page exists.

No open data portal, no documented course/SIS API, no `llms.txt`, no `/.well-known/security.txt` and no status page were found on any WashU host. No endpoints were fabricated, and no contract was saved for any surface whose operator is a vendor.

## Maintainers

- Kin Lane — kin@apievangelist.com
