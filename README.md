# Cloverly (cloverly)

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

Cloverly is an Atlanta-headquartered climate technology company that operates a developer-first carbon-credit infrastructure platform. The Cloverly API estimates and purchases verified carbon offsets in real time across a curated portfolio of reforestation, biochar, direct air capture, renewable energy, and methane-abatement projects sourced from registries such as Verra, Gold Standard, ACR, Climate Action Reserve, and Puro.earth. The Catalyst product extends the same platform to project developers managing inventory, pricing, content, payments, and omnichannel distribution. In 2024 Cloverly was acquired by Climate Impact X (CIX), the Singapore-based carbon exchange, and has since operated as the technology arm powering CIX-aligned voluntary carbon market infrastructure.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/cloverly/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/cloverly/refs/heads/main/apis.yml)

## Scope

- **Access:** 3rd-Party

## Tags

- Carbon
- Carbon Credits
- Carbon Offsets
- Catalyst
- Climate
- Climate Action
- Climate Impact X
- CIX
- Decarbonization
- ESG
- Greenhouse Gas
- Net Zero
- Project Developers
- Registries
- Sustainability
- Voluntary Carbon Market
- VCM

## Timestamps

- **Created:** 2026-05-24
- **Modified:** 2026-05-24

## APIs

### Cloverly Estimates API

Create and retrieve carbon-offset estimates without committing a purchase. Supports shipping (distance + weight), vehicle (distance + fuel efficiency), flights (passenger-miles), electricity (kWh), direct carbon weight, and fixed currency amounts. Each estimate returns a slug, the equivalent carbon in grams, the matched offset source, and the transaction cost in USD cents, then can be converted to a purchase via the Purchases API.

- **Human URL:** [https://docs.cloverly.com](https://docs.cloverly.com)
- **Base URL:** `https://api.cloverly.com`

#### Tags

- Carbon
- Climate
- Estimates
- Offsets
- Sustainability

#### Properties

- [Documentation](https://docs.cloverly.com)
- [OpenAPI](openapi/cloverly-estimates-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/cloverly-estimates-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cloverly-estimates-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/cloverly-estimate-schema.json) — [JSON Schema](https://json-schema.org/specification)

### Cloverly Purchases API

Purchase and retire carbon offsets from Cloverly's curated marketplace. Mirrors the Estimates shape (shipping, vehicle, flight, electricity, carbon, currency) but immediately reserves and retires credits against a verified project. Estimates can be promoted to purchases by posting their slug.

- **Human URL:** [https://docs.cloverly.com](https://docs.cloverly.com)
- **Base URL:** `https://api.cloverly.com`

#### Tags

- Carbon
- Climate
- Purchases
- Offsets
- Retirement

#### Properties

- [Documentation](https://docs.cloverly.com)
- [OpenAPI](openapi/cloverly-purchases-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/cloverly-purchases-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cloverly-purchases-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/cloverly-purchase-schema.json) — [JSON Schema](https://json-schema.org/specification)

### Cloverly Offset Types API

List the carbon-offset project types and individual offset sources available through Cloverly — including reforestation, biochar, direct air capture, renewable energy, methane abatement, and other registry-backed projects. Each source records the registry (Verra, Gold Standard, ACR, Climate Action Reserve, Puro.earth, etc.), project location, vintage, available tonnes, and price per tonne.

- **Human URL:** [https://docs.cloverly.com](https://docs.cloverly.com)
- **Base URL:** `https://api.cloverly.com`

#### Tags

- Carbon
- Catalog
- Climate
- Offsets
- Projects

#### Properties

- [Documentation](https://docs.cloverly.com)
- [OpenAPI](openapi/cloverly-offset-types-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/cloverly-offset-types-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cloverly-offset-types-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Cloverly Account API

Retrieve the authenticated account record including the configured currency, default offset type preferences, and the public/private API key context. Useful for confirming which environment (sandbox vs production) and which key tier a client is operating under.

- **Human URL:** [https://docs.cloverly.com](https://docs.cloverly.com)
- **Base URL:** `https://api.cloverly.com`

#### Tags

- Account
- Carbon
- Climate

#### Properties

- [Documentation](https://docs.cloverly.com)
- [OpenAPI](openapi/cloverly-account-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/cloverly-account-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cloverly-account-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Portal](https://cloverly.com)
- [Documentation](https://docs.cloverly.com)
- [Sign Up](https://dashboard.cloverly.com)
- [Registration](https://dashboard.cloverly.com/user/new)
- [Product Page](https://cloverly.com/api)
- [Product Page](https://cloverly.com/catalyst)
- [Marketplace](https://supply.cloverly.com)
- [Blog](https://cloverly.com/blog)
- [Case Studies](https://cloverly.com/case-studies)
- [White Papers](https://cloverly.com/white-papers)
- [Contact Us](https://cloverly.com/contact)
- [Careers](https://cloverly.com/careers)
- [LinkedIn](https://www.linkedin.com/company/cloverly/)
- [Twitter](https://twitter.com/getcloverly)
- [YouTube](https://www.youtube.com/@getcloverly)
- [GitHub Organization](https://github.com/cloverly)
- [SDK](https://github.com/cloverly/cloverly-ruby-gem)
- [SDK](https://github.com/cloverly/cloverly-python-module)
- [Package Registry](https://rubygems.org/gems/cloverly)
- [Package Registry](https://pypi.org/project/cloverly-python-module/)
- [API Reference](https://docs.cloverly.com)
- [Plans](plans/cloverly-plans-pricing.yml)
- [Rate Limits](rate-limits/cloverly-rate-limits.yml)
- [Fin Ops](finops/cloverly-finops.yml)
- [Vocabulary](vocabulary/cloverly-vocabulary.yml)
- [JSON-LD](json-ld/cloverly-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Spectral Rules](rules/cloverly-rules.yml) — [Spectral](https://docs.stoplight.io/docs/spectral)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
