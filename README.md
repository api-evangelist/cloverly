# Cloverly (cloverly)

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
