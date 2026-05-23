# Bassetts Ice Cream

API Evangelist profile of [Bassetts Ice Cream](https://www.bassettsicecream.com) — a sixth-generation Philadelphia ice cream brand founded in 1861, self-described as "America's oldest ice cream brand," operating a single retail counter at Reading Terminal Market plus a regional wholesale frozen-dessert distribution business and a small international export footprint (China, South Korea, Taiwan).

This is a tiny regional consumer packaged goods (CPG) brand. **There is no public API, no developer portal, no documented webhooks, and no machine-readable product feed.** This repository captures the brand, product surface, distribution channels, and contact surface as structured data so it can be referenced by API Evangelist network indexes and downstream Naftiko governance / catalog systems.

## Tier 3 — No APIs

Classified `x-tier: 3` in the API Evangelist network registry with `x-tier-reason: no-apis`. The website is hosted on Wix; the only machine-readable surface is the Wix-generated `sitemap.xml`.

## At a Glance

- **Founded:** 1861, by Lewis Dubois Bassett
- **Current CEO:** Michael Strange, great-great-grandson of the founder
- **Sixth generation:** Eric Bassett (operations, catering) and Alex Strange
- **Retail:** Reading Terminal Market, 45 N. 12th Street, Philadelphia, PA — open 9am-6pm daily
- **Corporate:** 1211 Chestnut Street, Suite 410, Philadelphia, PA 19107
- **Direct wholesale radius:** 40 miles from Philadelphia
- **Distributor regions:** Greater New York, Florida
- **International:** China (since 2008), South Korea (since 2017), Taiwan (since 2020)
- **Nationwide DTC:** via [Goldbelly](https://www.goldbelly.com)

## Product Surface

| Line | Examples |
|---|---|
| Classic flavors | Vanilla (Madagascar Bourbon), French Vanilla, Chocolate (Dutch cocoa), Dark Chocolate |
| Premium flavors | Butterscotch Vanilla, Mint Chocolate Chip, Coffee, Peanut Butter Swirl, Moose Tracks, English Toffee Crunch, Salted Caramel Pretzel |
| Seasonal / fruit | Pumpkin, Cherry Vanilla, Mango, Peach, Strawberry, Pistachio |
| Sorbets | Lemon, Mango-Apricot, Raspberry |
| Novelties | Ice cream bars, ice cream sandwiches |
| Wholesale formats | 2.5-gallon tubs (Bassetts), 3-gallon tubs (Turkey Hill, Kemps, premium bulk), 8-pint cases, soft-serve 4 oz insulated cups |
| Distributed third-party | Turkey Hill Ice Cream, Kemps Ice Cream, Georgeo's Italian Ices |

## Account Types Served (Wholesale)

Restaurants, dipping parlors, country clubs, hotels, supermarkets, caterers.

## Repository Contents

| Path | Purpose |
|---|---|
| [`apis.yml`](apis.yml) | APIs.json 0.18 index — common properties only (website, retail, wholesale, catering, distributors, social, contact). `apis: []`. |
| [`vocabulary/bassetts-ice-cream-vocabulary.yml`](vocabulary/bassetts-ice-cream-vocabulary.yml) | Brand, product, channel, account, and operational vocabulary. |
| [`json-ld/bassetts-ice-cream-context.jsonld`](json-ld/bassetts-ice-cream-context.jsonld) | Schema.org JSON-LD context modeling Bassetts as an `Organization`/`Brand` plus the Reading Terminal Market `IceCreamShop`. |

## Artifacts Intentionally Absent

| Artifact | Why absent |
|---|---|
| `openapi/` | No public HTTP API. |
| `asyncapi/` | No public event/messaging surface. |
| `capabilities/` | Nothing to compose — no API to call. |
| `rules/` | No OpenAPI to lint. |
| `json-schema/` / `json-structure/` | No machine-readable entity surface beyond what the JSON-LD context already names. |
| `examples/` | No request/response payloads exist. |
| `plans/` | No published pricing model — wholesale quoting is account-by-account; retail/Goldbelly pricing is unstructured. |
| `rate-limits/` | No API. |
| `finops/` | No API metering. |
| `crd/` | No Kubernetes resources. |

## Notable Sources

- Homepage and store info — <https://www.bassettsicecream.com>
- History — <https://www.bassettsicecream.com/our-history-1>
- About / ownership — <https://www.bassettsicecream.com/about-1>
- Flavor gallery — <https://www.bassettsicecream.com/flavor-gallery>
- Wholesale & products — <https://www.bassettsicecream.com/wholesale> · <https://www.bassettsicecream.com/wholesale-products-menu>
- International distribution — <https://www.bassettsicecream.com/international-1>
- Wix-generated sitemap — <https://www.bassettsicecream.com/sitemap.xml>

## Maintainer

[Kin Lane](https://apievangelist.com) — API Evangelist
