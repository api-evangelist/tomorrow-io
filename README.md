# Tomorrow.io (tomorrow-io)

Tomorrow.io is a Boston-based weather intelligence platform combining a global proprietary numerical weather model, a constellation of microsatellite weather radars, and a developer-facing v4 REST API. The platform exposes 60+ hyperlocal data layers — core weather, air quality, pollen, solar, soil, fire, flood, lightning, maritime, aviation, road — together with map tiles, severe-weather event detection, routable forecast queries, climate normals, historical archive access, customer-defined locations, named insights, and threshold-based webhook alerts. Used by airlines, on-demand logistics platforms, agriculture, energy, and the US Air Force, Tomorrow.io's API is designed for ETA-aware route planning, geofenced alerting, agentic workflows, and large-scale operational decisioning under weather risk.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/tomorrow-io/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/tomorrow-io/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Access:** 3rd-Party

## Tags

- Weather
- Forecast
- Climate
- Risk
- Air Quality
- Pollen
- Lightning
- Severe Weather
- Maps
- Routing
- Satellite
- Microsatellites
- Radar
- Geospatial
- Alerts

## Timestamps

- **Created:** 2026-05-24
- **Modified:** 2026-05-24

## APIs

### Tomorrow.io Weather API

Realtime conditions, 14-day forecast (minutely, hourly, daily), and flexible timeline retrieval across the full Tomorrow.io 60+ data-layer catalog for any point, polygon, or polyline on Earth.

- **Human URL:** [https://docs.tomorrow.io/reference/welcome](https://docs.tomorrow.io/reference/welcome)
- **Base URL:** `https://api.tomorrow.io/v4`

#### Tags

- Weather
- Realtime
- Forecast
- Timelines

#### Properties

- [Documentation](https://docs.tomorrow.io/reference/welcome)
- [API Reference](https://docs.tomorrow.io/reference/realtime-weather)
- [API Reference](https://docs.tomorrow.io/reference/weather-forecast)
- [API Reference](https://docs.tomorrow.io/reference/timelines-overview)
- [OpenAPI](openapi/tomorrow-io-weather-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tomorrow-io-weather-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tomorrow-io-weather-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/tomorrow-io-weather-values-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/tomorrow-io-weather-values-structure.json)
- [Example](examples/tomorrow-io-realtime-example.json)
- [Example](examples/tomorrow-io-timelines-example.json)

### Tomorrow.io Historical Weather API

Retrieve historical weather observations and monthly climate normals for any point or polygon on Earth using the same field catalog as the realtime and forecast APIs.

- **Human URL:** [https://docs.tomorrow.io/reference/historical](https://docs.tomorrow.io/reference/historical)
- **Base URL:** `https://api.tomorrow.io/v4`

#### Tags

- Weather
- Historical
- Climate
- Climate Normals

#### Properties

- [Documentation](https://docs.tomorrow.io/reference/historical)
- [API Reference](https://docs.tomorrow.io/reference/historical-weather-retrieval)
- [API Reference](https://docs.tomorrow.io/reference/climate-normals)
- [OpenAPI](openapi/tomorrow-io-historical-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tomorrow-io-historical-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tomorrow-io-historical-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Tomorrow.io Events API

Retrieve severe weather events, fires, floods, lightning swarms, and custom vector events affecting a point or geometry.

- **Human URL:** [https://docs.tomorrow.io/reference/retrieve-events-basic](https://docs.tomorrow.io/reference/retrieve-events-basic)
- **Base URL:** `https://api.tomorrow.io/v4`

#### Tags

- Weather
- Events
- Severe Weather
- Lightning
- Floods
- Fire

#### Properties

- [API Reference](https://docs.tomorrow.io/reference/retrieve-events-basic)
- [Documentation](https://docs.tomorrow.io/reference/severe-weather-events)
- [OpenAPI](openapi/tomorrow-io-events-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tomorrow-io-events-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tomorrow-io-events-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/tomorrow-io-event-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Example](examples/tomorrow-io-events-example.json)

### Tomorrow.io Weather on Routes API

Retrieve weather along an arbitrary polyline of waypoints at the times each segment is expected to be traversed — powers route optimization, logistics planning, and ETA-aware hazard detection.

- **Human URL:** [https://docs.tomorrow.io/reference/route](https://docs.tomorrow.io/reference/route)
- **Base URL:** `https://api.tomorrow.io/v4`

#### Tags

- Weather
- Route
- Logistics
- ETA

#### Properties

- [API Reference](https://docs.tomorrow.io/reference/route)
- [OpenAPI](openapi/tomorrow-io-route-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tomorrow-io-route-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tomorrow-io-route-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Example](examples/tomorrow-io-route-example.json)

### Tomorrow.io Weather Maps API

Web Mercator (XYZ) PNG tile service for rendering Tomorrow.io weather data layers — precipitation radar, temperature, wind, clouds, air quality — directly into Mapbox, MapLibre, Leaflet, OpenLayers, or Google Maps.

- **Human URL:** [https://docs.tomorrow.io/reference/map-overview](https://docs.tomorrow.io/reference/map-overview)
- **Base URL:** `https://api.tomorrow.io/v4`

#### Tags

- Weather
- Maps
- Tiles
- Visualization

#### Properties

- [Documentation](https://docs.tomorrow.io/reference/map-overview)
- [API Reference](https://docs.tomorrow.io/reference/retrieve-a-tile-basic)
- [OpenAPI](openapi/tomorrow-io-map-tiles-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tomorrow-io-map-tiles-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tomorrow-io-map-tiles-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Tomorrow.io Locations API

Manage saved locations (points, polygons, lines) referenced by ``locationId`` across the Tomorrow.io APIs, with tag-based cohorts for fleet, customer, or asset organization.

- **Human URL:** [https://docs.tomorrow.io/reference/list-locations](https://docs.tomorrow.io/reference/list-locations)
- **Base URL:** `https://api.tomorrow.io/v4`

#### Tags

- Weather
- Locations
- Geometry

#### Properties

- [API Reference](https://docs.tomorrow.io/reference/list-locations)
- [OpenAPI](openapi/tomorrow-io-locations-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tomorrow-io-locations-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tomorrow-io-locations-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/tomorrow-io-location-schema.json) — [JSON Schema](https://json-schema.org/specification)

### Tomorrow.io Alerts API

Create and manage threshold-based weather alerts that evaluate Tomorrow.io data layers against custom rules for linked locations and deliver notifications via webhook, email, and the Tomorrow.io app.

- **Human URL:** [https://docs.tomorrow.io/reference/create-alerts](https://docs.tomorrow.io/reference/create-alerts)
- **Base URL:** `https://api.tomorrow.io/v4`

#### Tags

- Weather
- Alerts
- Webhooks
- Notifications

#### Properties

- [API Reference](https://docs.tomorrow.io/reference/create-alerts)
- [OpenAPI](openapi/tomorrow-io-alerts-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tomorrow-io-alerts-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tomorrow-io-alerts-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/tomorrow-io-alert-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Example](examples/tomorrow-io-alert-example.json)

### Tomorrow.io Insights API

Define and manage reusable Insights — named rules combining Tomorrow.io data layers, operators, and thresholds — that power the Events and Alerts APIs.

- **Human URL:** [https://docs.tomorrow.io/reference/list-insights](https://docs.tomorrow.io/reference/list-insights)
- **Base URL:** `https://api.tomorrow.io/v4`

#### Tags

- Weather
- Insights
- Rules

#### Properties

- [API Reference](https://docs.tomorrow.io/reference/list-insights)
- [OpenAPI](openapi/tomorrow-io-insights-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tomorrow-io-insights-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tomorrow-io-insights-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/tomorrow-io-insight-schema.json) — [JSON Schema](https://json-schema.org/specification)

## Common Properties

- [Arazzo Workflows](arazzo/) — [Arazzo Specification](https://spec.openapis.org/arazzo/latest.html)
- [Portal](https://www.tomorrow.io)
- [Documentation](https://docs.tomorrow.io)
- [API Reference](https://docs.tomorrow.io/reference/welcome)
- [Authentication](https://app.tomorrow.io/development/keys)
- [Sign Up](https://app.tomorrow.io/signup)
- [Console](https://app.tomorrow.io/signin)
- [Sandbox](https://docs.tomorrow.io/recipes)
- [Getting Started](https://docs.tomorrow.io/reference/getting-started)
- [Rate Limits](https://docs.tomorrow.io/reference/rate-limiting)
- [Errors](https://docs.tomorrow.io/reference/error-handling)
- [Changelog](https://docs.tomorrow.io/reference/release-notes)
- [Documentation](https://docs.tomorrow.io/llms.txt)
- [Documentation](https://docs.tomorrow.io/reference/tomorrow-io-mcp)
- [Pricing](https://www.tomorrow.io/pricing/)
- [Terms of Service](https://www.tomorrow.io/legal/tos/)
- [Privacy Policy](https://www.tomorrow.io/legal/privacy-policy/)
- [Support](https://support.tomorrow.io)
- [Blog](https://www.tomorrow.io/blog/)
- [GitHub Organization](https://github.com/Tomorrow-IO-API)
- [SDK](https://github.com/Tomorrow-IO-API/tomorrow-postman)
- [SDK](https://github.com/Tomorrow-IO-API/tomorrow-samples)
- [SDK](https://github.com/Tomorrow-IO-API/tomorrow-route-mapbox)
- [SDK](https://github.com/Tomorrow-IO-API/tomorrow-timelines-widget)
- [SDK](https://github.com/Tomorrow-IO-API/tomorrow-events-charts)
- [SDK](https://github.com/Tomorrow-IO-API/tomorrow-api-proxy)
- [SDK](https://github.com/Tomorrow-IO-API/tomorrow-netlify)
- [SDK](https://github.com/Tomorrow-IO-API/tomorrow-map-spectrums)
- [SDK](https://github.com/Tomorrow-IO-API/tomorrow-weather-codes)
- [SDK](https://github.com/Tomorrow-IO-API/climate-normals)
- [LinkedIn](https://www.linkedin.com/company/tomorrow-io)
- [Twitter](https://twitter.com/tomorrow_io)
- [Spectral Rules](rules/tomorrow-io-rules.yml)
- [Vocabulary](vocabulary/tomorrow-io-vocabulary.yml)
- [JSON-LD](json-ld/tomorrow-io-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Plans](plans/tomorrow-io-plans-pricing.yml)
- [Rate Limits](rate-limits/tomorrow-io-rate-limits.yml)
- [Fin Ops](finops/tomorrow-io-finops.yml)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)
- [Solutions](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
