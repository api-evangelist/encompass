# Encompass (encompass)

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
