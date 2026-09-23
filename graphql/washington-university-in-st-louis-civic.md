# CIViC GraphQL API — Washington University in St. Louis

```yaml
x-method: derived
generated: '2026-09-01'
method: probed
x-source-url: https://docs.civicdb.org/en/latest/api.html
x-authorship: >-
  This overview is our writing. The schema file beside it is CIViC's own document,
  harvested from the live endpoint by introspection.
```

- **provider:** Washington University in St. Louis (`washington-university-in-st-louis`)
- **operator:** `institution`
- **generated:** 2026-09-01
- **method:** probed
- **source:** live GraphQL introspection against `https://civicdb.org/api/graphql`, plus the
  operator's own documentation at `https://docs.civicdb.org/en/latest/api.html`

## Why this is Washington University's, and not a vendor's

CIViC — the Clinical Interpretation of Variants in Cancer knowledgebase — is not a product
Washington University bought. Its own documentation footer states it plainly:

> CIViC by The McDonnell Genome Institute at Washington University School of Medicine is licensed
> under a Creative Commons Public Domain Dedication (CC0 1.0 Universal)

The API runs on an independent project domain (`civicdb.org`, nameservers on Google Cloud), which
is why a hostname-only verdict cannot see it. Judged the way STEP 0c of the enrichment contract
requires — by what the contract and its documentation say about themselves — the operator is the
institution. This is one of the very few genuinely public, institution-engineered APIs in the
university cohort.

## Endpoint

| | |
|---|---|
| GraphQL endpoint | `https://civicdb.org/api/graphql` |
| Interactive explorer | `https://civicdb.org/api/graphiql` |
| Documentation | `https://docs.civicdb.org/en/latest/api.html` |
| Source | `https://github.com/griffithlab/civic-v2` |
| License | CC0 1.0 Universal |

The previous REST ("V1") API is documented by the operator as **deprecated and no longer
available**. GraphQL is the only live contract.

## Authentication

Anonymous reads are permitted. Mutations, and any request that should escape the anonymous rate
limit, carry a CIViC API key as an HTTP bearer token:

```
Authorization: Bearer <CIVIC_API_KEY>
```

Keys are generated from a signed-in user profile (*Manage API Keys*), shown once at creation, and
revocable. The operator explicitly documents that keys must not be placed in URLs, query strings,
checked-in scripts or shared notebooks.

## Rate limits

Documented by the operator: **3 requests/second measured over a 5-minute window**, burstable above
that rate for short periods. An API key is free and raises the anonymous ceiling. The operator
directs high-throughput or continuous consumers to CIViCpy rather than the live endpoint.

## Schema shape (as introspected 2026-09-01)

| | |
|---|---|
| Total named types | 502 |
| Objects | 271 |
| Input objects | 137 |
| Enums | 73 |
| Interfaces | 9 |
| Unions | 5 |
| Root `Query` fields | 112 |
| Root `Mutation` fields | 47 |

### Domain coverage

- **Molecular profiles and variants** — `browseMolecularProfiles`, `browseVariants`,
  `variantGroup`, `cytogeneticRegion`, fusion / region / factor variant families
- **Features and genes** — `browseFeatures`, `feature`, `featureTypeahead`
- **Evidence and assertions** — `evidenceItems`, `assertions`, `approvals`, the curation
  revision model (`suggest*Revision`, `acceptRevisions`, `rejectRevisions`)
- **Clinical context** — `diseases`, `therapies`, `phenotypes`, `clinicalTrials`, ACMG and
  ClinGen code vocabularies
- **Sources and provenance** — `browseSources`, `addRemoteCitation`, `suggestSource`,
  `dataReleases`
- **Community** — `browseUsers`, `browseOrganizations`, `contributors`, `comments`, `events`,
  `activities`, subscription and notification handling

### Curation as a write surface

The 47 mutations are unusual for an academic knowledgebase: CIViC exposes its whole expert
crowdsourcing workflow through the API — submit evidence, suggest revisions, moderate and approve
assertions, flag and resolve entities, and manage the caller's own API keys
(`generateApiKey`, `revokeApiKey`). That makes it a read *and* write contract, not a data dump.

## Files

- `washington-university-in-st-louis-civic-schema.graphql` — the full SDL, printed directly from
  the introspection response. Nothing in it is hand-authored.
