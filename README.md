# Cloverly (cloverly)

Cloverly is an Atlanta-headquartered climate technology company that operates a developer-first carbon-credit infrastructure platform. The Cloverly API estimates and purchases verified carbon offsets in real time across a curated portfolio of reforestation, biochar, direct air capture, renewable energy, and methane-abatement projects sourced from registries such as Verra, Gold Standard, ACR, Climate Action Reserve, and Puro.earth. The Catalyst product extends the same platform to project developers managing inventory, pricing, content, payments, and omnichannel distribution. In 2024 Cloverly was acquired by Climate Impact X (CIX), the Singapore-based carbon exchange, and has since operated as the technology arm powering CIX-aligned voluntary carbon market infrastructure.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/cloverly/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

 - Carbon, Carbon Credits, Carbon Offsets, Catalyst, Climate, Climate Action, Climate Impact X, CIX, Decarbonization, ESG, Greenhouse Gas, Net Zero, Project Developers, Registries, Sustainability, Voluntary Carbon Market, VCM

## Timestamps

- **Created:** 2026-05-24
- **Modified:** 2026-05-24

## APIs

### Cloverly Estimates API
Create and retrieve carbon-offset estimates without committing a purchase. Activity types: shipping (distance + weight), vehicle (distance + fuel efficiency), flights (passenger-miles), electricity (kWh), direct carbon weight, and fixed currency amounts. Each estimate returns a slug, total CO2e in grams, the matched offset source, and the transaction cost in USD cents.

**Human URL:** [https://docs.cloverly.com](https://docs.cloverly.com)

- [Documentation](https://docs.cloverly.com)
- [OpenAPI](openapi/cloverly-estimates-api-openapi.yml)
- [JSON Schema — Estimate](json-schema/cloverly-estimate-schema.json)
- [Naftiko Capability — Estimates](capabilities/estimates-estimates.yaml)

### Cloverly Purchases API
Purchase and retire carbon offsets from Cloverly's curated marketplace. Mirrors the Estimates shape (shipping, vehicle, flight, electricity, carbon, currency) but immediately reserves and retires credits against a verified project. Estimates can be promoted to purchases by posting their slug to `/purchases`.

**Human URL:** [https://docs.cloverly.com](https://docs.cloverly.com)

- [Documentation](https://docs.cloverly.com)
- [OpenAPI](openapi/cloverly-purchases-api-openapi.yml)
- [JSON Schema — Purchase](json-schema/cloverly-purchase-schema.json)
- [Naftiko Capability — Purchases](capabilities/purchases-purchases.yaml)

### Cloverly Offset Types API
List the carbon-offset project types and individual offset sources available through Cloverly — reforestation, biochar, direct air capture, renewable energy, methane abatement, and other registry-backed projects. Each source records the registry (Verra, Gold Standard, ACR, CAR, Puro.earth), project location, vintage, available tonnes, and price per tonne.

**Human URL:** [https://docs.cloverly.com](https://docs.cloverly.com)

- [Documentation](https://docs.cloverly.com)
- [OpenAPI](openapi/cloverly-offset-types-api-openapi.yml)
- [Naftiko Capability — Offset Types](capabilities/offset-types-offset-types.yaml)

### Cloverly Account API
Retrieve the authenticated account record including the configured currency, default offset preferences, and the public/private API key context.

**Human URL:** [https://docs.cloverly.com](https://docs.cloverly.com)

- [Documentation](https://docs.cloverly.com)
- [OpenAPI](openapi/cloverly-account-api-openapi.yml)
- [Naftiko Capability — Account](capabilities/account-account.yaml)

## Common Properties

- [Portal — cloverly.com](https://cloverly.com)
- [Documentation — docs.cloverly.com](https://docs.cloverly.com)
- [ProductPage — API](https://cloverly.com/api)
- [ProductPage — Catalyst](https://cloverly.com/catalyst)
- [Marketplace — Supply](https://supply.cloverly.com)
- [SignUp — Dashboard](https://dashboard.cloverly.com)
- [Registration](https://dashboard.cloverly.com/user/new)
- [Blog](https://cloverly.com/blog)
- [CaseStudies](https://cloverly.com/case-studies)
- [WhitePapers](https://cloverly.com/white-papers)
- [ContactUs](https://cloverly.com/contact)
- [Careers](https://cloverly.com/careers)
- [LinkedIn](https://www.linkedin.com/company/cloverly/)
- [Twitter](https://twitter.com/getcloverly)
- [YouTube](https://www.youtube.com/@getcloverly)
- [GitHubOrganization](https://github.com/cloverly)
- [SDK — Ruby Gem](https://github.com/cloverly/cloverly-ruby-gem)
- [SDK — Python Module](https://github.com/cloverly/cloverly-python-module)
- [PackageRegistry — RubyGems](https://rubygems.org/gems/cloverly)
- [PackageRegistry — PyPI](https://pypi.org/project/cloverly-python-module/)

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Cloverly Estimates API](openapi/cloverly-estimates-api-openapi.yml)
- [Cloverly Purchases API](openapi/cloverly-purchases-api-openapi.yml)
- [Cloverly Offset Types API](openapi/cloverly-offset-types-api-openapi.yml)
- [Cloverly Account API](openapi/cloverly-account-api-openapi.yml)

### JSON Schema

- [Cloverly Estimate Schema](json-schema/cloverly-estimate-schema.json)
- [Cloverly Purchase Schema](json-schema/cloverly-purchase-schema.json)

### JSON Structure

- [Cloverly Estimate Structure](json-structure/cloverly-estimate-structure.json)

### JSON-LD

- [Cloverly Context](json-ld/cloverly-context.jsonld)

### Examples

- [Estimate Shipping](examples/cloverly-estimate-shipping-example.json)
- [Convert Estimate To Purchase](examples/cloverly-purchase-conversion-example.json)
- [List Offset Sources](examples/cloverly-list-offsets-example.json)

### Capabilities (Naftiko)

- [Estimates](capabilities/estimates-estimates.yaml)
- [Purchases](capabilities/purchases-purchases.yaml)
- [Offset Types](capabilities/offset-types-offset-types.yaml)
- [Account](capabilities/account-account.yaml)
- [Cloverly Platform Workflow](capabilities/cloverly-platform.yaml)

### Rules (Spectral)

- [Cloverly Rules](rules/cloverly-rules.yml)

### Vocabulary

- [Cloverly Vocabulary](vocabulary/cloverly-vocabulary.yml)

### Commercial artifacts

- [Plans / Pricing](plans/cloverly-plans-pricing.yml)
- [Rate Limits](rate-limits/cloverly-rate-limits.yml)
- [FinOps Definition](finops/cloverly-finops.yml)

## Maintainers

**FN:** Kin Lane

**Email:** info@apievangelist.com
