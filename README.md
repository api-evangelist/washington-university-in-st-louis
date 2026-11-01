# Washington University in St. Louis

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

Washington University in St. Louis (WashU) is a private research university in St. Louis, Missouri, now presenting itself on washu.edu with the historic wustl.edu domain redirecting to it. Its programmable footprint is small but, unusually for this cohort, not empty and not entirely someone else's: the McDonnell Genome Institute at WashU School of Medicine builds and operates CIViC, the Clinical Interpretation of Variants in Cancer knowledgebase, whose public GraphQL API at civicdb.org/api/graphql answers anonymous introspection with a 502-type schema, 112 root queries and 47 mutations, documents a bearer-token API key and a 3 request/second rate limit, and is released CC0. WashU also operates its own Shibboleth SAML 2.0 identity provider, published as signed metadata in InCommon with REFEDS Research & Scholarship and SIRTFI assurance — machine readable institutional infrastructure almost no university in this cohort catalogues. Its enterprise integration APIs (Person, Financial, Supplier, Location, Academic, Organization) are real but wholly gated: they live in a MuleSoft Anypoint Exchange tenant and access is granted by internal ServiceNow request, with no public specification, endpoint or sign-up. Everything else is a relationship rather than WashU engineering. The two research repositories that harvest cleanly over OAI-PMH 2.0 — the WashU Scholarly Repository and Digital Commons Data@Becker — both sit on wustl.edu hostnames that CNAME straight to Elsevier infrastructure (bepress and Mendeley Data), so the data and the DOIs are WashU's and the contracts are Elsevier's. WashU is a DataCite direct member with two registered repositories. There is no public open-data portal, no documented course or SIS API, and courses.wustl.edu no longer answers at all.

**Areas:** University · Higher Education · Education · United States · Missouri · Private Research University · Research Data · Research Repository · Identity Federation · Genomics · Bioinformatics · GraphQL

## Washington University in St. Louis on APIs.io

Everything profiled for Washington University in St. Louis is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/washington-university-in-st-louis/](https://apis.io/providers/washington-university-in-st-louis/)** — or go straight to one of the APIs or properties below.

### APIs (10)

- [CIViC — Clinical Interpretation of Variants in Cancer](https://apis.io/apis/washington-university-in-st-louis/civic/) — A free, open, community-curated knowledgebase of the clinical significance of variants in cancer, built and operated by The McDonnell Genome Institute at…
- [WashU Enterprise Integration APIs (MuleSoft Anypoint)](https://apis.io/apis/washington-university-in-st-louis/enterprise-apis/) — Institutional integration APIs published in a MuleSoft Anypoint Exchange tenant and described publicly as "Data at WashU", covering the Person, Financial,…
- [WashU Shibboleth Identity Provider (InCommon)](https://apis.io/apis/washington-university-in-st-louis/incommon-idp/) — Washington University's own SAML 2.0 identity provider, entityID https://login.wustl.edu/idp/shibboleth, published as signed metadata through the InCommon…
- [WashU Scholarly Repository (OAI-PMH)](https://apis.io/apis/washington-university-in-st-louis/open-scholarship/) — The university's institutional repository, "WashU Scholarly Repository", serving a live OAI-PMH 2.0 interface with nine metadata formats including oai_etdms…
- [Digital Commons Data@Becker (Research Data Repository)](https://apis.io/apis/washington-university-in-st-louis/digital-commons-data/) — The Becker Medical Library and School of Medicine research data repository, publishing an API documentation page and a live OAI-PMH 2.0 endpoint that serves…
- [DataCite Membership — Washington University in St. Louis Libraries](https://apis.io/apis/washington-university-in-st-louis/datacite/) — Washington University in St. Louis Libraries is a DataCite direct member, symbol WUSTL, registered 2018-08-30, region AMER, and linked from DataCite's own…
- [ROR Registration — Washington University in St. Louis](https://apis.io/apis/washington-university-in-st-louis/ror/) — The institution's Research Organization Registry record, https://ror.org/01yc7t268, carrying its display name, multilingual name variants, the WUSTL…
- [Washington University in St. Louis Website (WordPress REST)](https://apis.io/apis/washington-university-in-st-louis/washu-edu-website-wordpress-rest/) — The public WordPress REST API (wp-json) of the Washington University in St. Louis website at washu.edu: the route index of the site's content management…
- [CNDA — Central Neuroimaging Data Archive (XNAT)](https://apis.io/apis/washington-university-in-st-louis/cnda/) — WashU's neuroimaging data archive, running XNAT — imaging informatics software that originated at the university's own Neuroinformatics Research Group.…
- [BALSA Neuroimaging Database](https://apis.io/apis/washington-university-in-st-louis/balsa/) — A WashU-operated database of neuroimaging scenes and datasets at balsa.wustl.edu, and now the destination of db.humanconnectome.org, which CNAMEs to…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### GraphQL (1)

GraphQL schemas.

- [CIViC GraphQL API — Washington University in St. Louis](https://apis.io/graphqls/washington-university-in-st-louis/washington-university-in-st-louis-civic/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Washington University In St Louis Context](https://apis.io/jsonld/washington-university-in-st-louis/washington-university-in-st-louis-context/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Washington University In St Louis Authentication](https://apis.io/security/washington-university-in-st-louis/washington-university-in-st-louis-authentication/)
- [Washington University In St Louis Domain Security](https://apis.io/security/washington-university-in-st-louis/washington-university-in-st-louis-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Washington University In St Louis Plans Pricing](https://apis.io/plans/washington-university-in-st-louis/washington-university-in-st-louis-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Washington University In St Louis Rate Limits](https://apis.io/rate-limits/washington-university-in-st-louis/washington-university-in-st-louis-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Washington University In St Louis Finops](https://apis.io/finops/washington-university-in-st-louis/washington-university-in-st-louis-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://washu.edu)
- [Documentation](https://data.wustl.edu/api-portal/)
- [API reference](https://docs.civicdb.org/en/latest/api.html)
- [Support](https://it.washu.edu/)
- [Blog](https://source.washu.edu/)
- [Privacy policy](https://registrar.washu.edu/student-records-resources/ferpa-overview/)
- [GitHub](https://github.com/WashU-IT-RIS)

## API Evangelist rating

**Kin Score 38.5** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 53.6 |
| Contract quality | 48.6 |
| Contract governance | 0.0 |
| Operational transparency | 34.2 |
| Developer ergonomics | 52.4 |
| Access clarity | 28.9 |

**Agent readiness 18.0** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | — |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 20.6** — Education & Research

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/washington-university-in-st-louis/](https://apis.io/providers/washington-university-in-st-louis/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Washington University in St. Louis: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/washington-university-in-st-louis/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
