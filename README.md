# Encompass (encompass)

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

Encompass is the dominant mortgage loan origination system (LOS), a product of **ICE Mortgage Technology** (formerly **Ellie Mae**, acquired by Intercontinental Exchange / ICE in 2020). Its developer program, **Encompass Developer Connect**, exposes REST APIs that let partners and lenders configure, customize, and administer loan information and resources programmatically — loan manufacturing, loan pipeline, borrower pairs, contacts, eFolder documents and attachments, milestones, conditions, users, and event webhooks.

Access is **partner/tenant-gated**: every call carries an OAuth 2.0 bearer token (`POST https://api.elliemae.com/oauth2/v1/token`) scoped to a specific Encompass instance, using a Client ID / secret / API key that a super-administrator persona provisions in the developer portal. The API reference is publicly browsable at [developer.icemortgagetechnology.com](https://developer.icemortgagetechnology.com/developer-connect/docs/welcome), though the interactive "try it" builder and actual calls require instance credentials. Versioning is path-based (v3 current; v1/v2 deprecated). The `api.elliemae.com` host still reflects the Ellie Mae lineage.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/encompass/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/encompass/refs/heads/main/apis.yml)

## Tags

- Mortgage
- Loan Origination
- LOS
- Fintech
- ICE Mortgage Technology
- Ellie Mae
- Lending

## Timestamps

- **Created:** 2026-07-04
- **Modified:** 2026-07-04

## APIs

### Encompass Loan Management API

Create, read, update, and delete Encompass loan files and read/write loan data fields between applications and Encompass, including moving loans between folders and retrieving UCD field definitions.

- **Human URL:** [https://developer.icemortgagetechnology.com/developer-connect/reference/loan-management](https://developer.icemortgagetechnology.com/developer-connect/reference/loan-management)
- **Base URL:** `https://api.elliemae.com`

#### Tags

- Loans
- Loan Data
- Loan Manufacturing

#### Properties

- [Documentation](https://developer.icemortgagetechnology.com/developer-connect/docs/welcome)
- [API Reference](https://developer.icemortgagetechnology.com/developer-connect/reference/loan-management)
- [OpenAPI](openapi/encompass-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/encompass.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/encompass.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Encompass Loan Pipeline API

Search for loans and loan fields across the pipeline using canonical field names, filter criteria, and cursor-based pagination for large result sets.

- **Human URL:** [https://developer.icemortgagetechnology.com/developer-connect/reference/loan-pipeline](https://developer.icemortgagetechnology.com/developer-connect/reference/loan-pipeline)
- **Base URL:** `https://api.elliemae.com`

#### Tags

- Pipeline
- Search
- Reporting

#### Properties

- [API Reference](https://developer.icemortgagetechnology.com/developer-connect/reference/loan-pipeline)
- [OpenAPI](openapi/encompass-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/encompass.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/encompass.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Encompass Borrower Pair & Applications API

Manage borrower pairs (applications) within a loan file — the borrower/co-borrower application entities that carry each borrower's data on a loan. *(Modeled from documented path conventions.)*

- **Human URL:** [https://developer.icemortgagetechnology.com/developer-connect/reference/loan-management](https://developer.icemortgagetechnology.com/developer-connect/reference/loan-management)
- **Base URL:** `https://api.elliemae.com`

#### Tags

- Borrowers
- Applications
- Borrower Pairs

#### Properties

- [API Reference](https://developer.icemortgagetechnology.com/developer-connect/reference/loan-management)
- [OpenAPI](openapi/encompass-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/encompass.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/encompass.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Encompass Contacts API

Manage borrower (consumer) contacts and business (service provider / vendor) contacts, including notes and groupings. *(Modeled from documented path conventions.)*

- **Human URL:** [https://developer.icemortgagetechnology.com/developer-connect/reference/browse-apis](https://developer.icemortgagetechnology.com/developer-connect/reference/browse-apis)
- **Base URL:** `https://api.elliemae.com`

#### Tags

- Contacts
- Borrower Contacts
- Business Contacts

#### Properties

- [API Reference](https://developer.icemortgagetechnology.com/developer-connect/reference/browse-apis)
- [OpenAPI](openapi/encompass-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/encompass.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/encompass.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Encompass eFolder Documents & Attachments API

Manage documents, attachments, and comments in a loan's eFolder — list and create document placeholders, and upload/retrieve attachments via cloud-storage URLs. V3 is current; several v1 attachment endpoints are being deprecated.

- **Human URL:** [https://developer.icemortgagetechnology.com/developer-connect/reference/efolder-document-1](https://developer.icemortgagetechnology.com/developer-connect/reference/efolder-document-1)
- **Base URL:** `https://api.elliemae.com`

#### Tags

- Documents
- eFolder
- Attachments

#### Properties

- [API Reference (Documents)](https://developer.icemortgagetechnology.com/developer-connect/reference/efolder-document-1)
- [API Reference (Attachments)](https://developer.icemortgagetechnology.com/developer-connect/reference/efolder-attachment-1)
- [OpenAPI](openapi/encompass-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/encompass.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/encompass.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Encompass Milestones & Associates API

Read and manage the milestones that mark a loan's progress through origination, complete/finish milestones, and assign the associates responsible at each stage. *(Modeled from documented path conventions.)*

- **Human URL:** [https://developer.icemortgagetechnology.com/developer-connect/reference/browse-apis](https://developer.icemortgagetechnology.com/developer-connect/reference/browse-apis)
- **Base URL:** `https://api.elliemae.com`

#### Tags

- Milestones
- Workflow
- Associates

#### Properties

- [API Reference](https://developer.icemortgagetechnology.com/developer-connect/reference/browse-apis)
- [OpenAPI](openapi/encompass-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/encompass.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/encompass.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Encompass Conditions API

Track and manage underwriting, preliminary, and post-closing conditions on a loan, including the modern Enhanced Conditions system. *(Modeled from documented path conventions.)*

- **Human URL:** [https://developer.icemortgagetechnology.com/developer-connect/reference/browse-apis](https://developer.icemortgagetechnology.com/developer-connect/reference/browse-apis)
- **Base URL:** `https://api.elliemae.com`

#### Tags

- Conditions
- Underwriting
- Tracking

#### Properties

- [API Reference](https://developer.icemortgagetechnology.com/developer-connect/reference/browse-apis)
- [OpenAPI](openapi/encompass-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/encompass.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/encompass.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Encompass Users API

Manage the internal Encompass users of a lender's instance — list, read, create, and update user accounts, personas, roles, and organization assignments. *(Modeled from documented path conventions.)*

- **Human URL:** [https://developer.icemortgagetechnology.com/developer-connect/reference/browse-apis](https://developer.icemortgagetechnology.com/developer-connect/reference/browse-apis)
- **Base URL:** `https://api.elliemae.com`

#### Tags

- Users
- Identity
- Administration

#### Properties

- [API Reference](https://developer.icemortgagetechnology.com/developer-connect/reference/browse-apis)
- [OpenAPI](openapi/encompass-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/encompass.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/encompass.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Encompass Webhooks API

Subscribe to Encompass resource events (loan created / updated / deleted / locked / unlocked and more), manage subscriptions, browse available resources and their events, query event history, and configure custom authentication for delivery. Push-based HTTP callbacks — **not** a bidirectional WebSocket.

- **Human URL:** [https://developer.icemortgagetechnology.com/developer-connect/reference/browse-apis](https://developer.icemortgagetechnology.com/developer-connect/reference/browse-apis)
- **Base URL:** `https://api.elliemae.com`

#### Tags

- Webhooks
- Events
- Subscriptions

#### Properties

- [API Reference](https://developer.icemortgagetechnology.com/developer-connect/reference/subscriptions)
- [OpenAPI](openapi/encompass-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/encompass.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/encompass.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/api-evangelist/encompass-developer-connect)
- [LinkedIn](https://www.linkedin.com/showcase/ice-mortgage-technology/)
- [Website](https://www.icemortgagetechnology.com/)
- [Documentation](https://developer.icemortgagetechnology.com/developer-connect/docs/welcome)
- [Plans](plans/encompass-plans-pricing.yml)
- [Rate Limits](rate-limits/encompass-rate-limits.yml)
- [Fin Ops](finops/encompass-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
