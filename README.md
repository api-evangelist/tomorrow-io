# Tomorrow.io (tomorrow-io)

Tomorrow.io is a Boston-based weather intelligence platform combining a global proprietary numerical weather model, a constellation of microsatellite weather radars, and a developer-facing v4 REST API. The platform exposes 60+ hyperlocal data layers — core weather, air quality, pollen, solar, soil, fire, flood, lightning, maritime, aviation, road — together with map tiles, severe-weather event detection, routable forecast queries, climate normals, historical archive access, customer-defined locations, named insights, and threshold-based webhook alerts. Used by airlines, on-demand logistics platforms, agriculture, energy, and the US Air Force, Tomorrow.io's API is designed for ETA-aware route planning, geofenced alerting, agentic workflows, and large-scale operational decisioning under weather risk.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/tomorrow-io/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

- Weather, Forecast, Climate, Risk, Air Quality, Pollen, Lightning, Severe Weather, Maps, Routing, Satellite, Microsatellites, Radar, Geospatial, Alerts

## Timestamps

- **Created:** 2026-05-24
- **Modified:** 2026-05-24

## Base URL

`https://api.tomorrow.io/v4`

Authenticated with the `apikey` query parameter. Sign up for a free key at [app.tomorrow.io](https://app.tomorrow.io/signup).

## APIs

### Tomorrow.io Weather API
Realtime conditions, 14-day forecast (minutely, hourly, daily), and flexible timeline retrieval across the full Tomorrow.io 60+ data-layer catalog for any point, polygon, or polyline on Earth.

**Human URL:** [https://docs.tomorrow.io/reference/welcome](https://docs.tomorrow.io/reference/welcome)

- [Documentation](https://docs.tomorrow.io/reference/welcome)
- [API Reference — Realtime](https://docs.tomorrow.io/reference/realtime-weather)
- [API Reference — Forecast](https://docs.tomorrow.io/reference/weather-forecast)
- [API Reference — Timelines](https://docs.tomorrow.io/reference/timelines-overview)
- [OpenAPI](openapi/tomorrow-io-weather-api-openapi.yml)
- [JSON Schema — Weather Values](json-schema/tomorrow-io-weather-values-schema.json)
- [JSON Structure — Weather Values](json-structure/tomorrow-io-weather-values-structure.json)
- [Example — Realtime](examples/tomorrow-io-realtime-example.json)
- [Example — Timelines](examples/tomorrow-io-timelines-example.json)
- [Naftiko Capability — Realtime Weather](capabilities/realtime-weather.yaml)
- [Naftiko Capability — Weather Forecast](capabilities/weather-forecast.yaml)
- [Naftiko Capability — Timelines](capabilities/timelines.yaml)

### Tomorrow.io Historical Weather API
Retrieve historical weather observations and monthly climate normals for any point or polygon on Earth using the same field catalog as the realtime and forecast APIs.

**Human URL:** [https://docs.tomorrow.io/reference/historical](https://docs.tomorrow.io/reference/historical)

- [Documentation](https://docs.tomorrow.io/reference/historical)
- [API Reference — Historical Retrieval](https://docs.tomorrow.io/reference/historical-weather-retrieval)
- [API Reference — Climate Normals](https://docs.tomorrow.io/reference/climate-normals)
- [OpenAPI](openapi/tomorrow-io-historical-api-openapi.yml)
- [Naftiko Capability — Historical Weather](capabilities/historical-weather.yaml)

### Tomorrow.io Events API
Retrieve severe weather events, fires, floods, lightning swarms, and custom vector events affecting a point or geometry.

**Human URL:** [https://docs.tomorrow.io/reference/retrieve-events-basic](https://docs.tomorrow.io/reference/retrieve-events-basic)

- [API Reference](https://docs.tomorrow.io/reference/retrieve-events-basic)
- [Severe Weather Events](https://docs.tomorrow.io/reference/severe-weather-events)
- [OpenAPI](openapi/tomorrow-io-events-api-openapi.yml)
- [JSON Schema — Event](json-schema/tomorrow-io-event-schema.json)
- [Example — Events](examples/tomorrow-io-events-example.json)
- [Naftiko Capability — Events](capabilities/events.yaml)

### Tomorrow.io Weather on Routes API
Retrieve weather along an arbitrary polyline of waypoints at the times each segment is expected to be traversed — powers route optimization, logistics planning, and ETA-aware hazard detection.

**Human URL:** [https://docs.tomorrow.io/reference/route](https://docs.tomorrow.io/reference/route)

- [API Reference](https://docs.tomorrow.io/reference/route)
- [OpenAPI](openapi/tomorrow-io-route-api-openapi.yml)
- [Example — Route](examples/tomorrow-io-route-example.json)
- [Naftiko Capability — Weather on Route](capabilities/weather-on-route.yaml)

### Tomorrow.io Weather Maps API
Web Mercator (XYZ) PNG tile service for rendering Tomorrow.io weather data layers directly into Mapbox, MapLibre, Leaflet, OpenLayers, or Google Maps.

**Human URL:** [https://docs.tomorrow.io/reference/map-overview](https://docs.tomorrow.io/reference/map-overview)

- [Documentation](https://docs.tomorrow.io/reference/map-overview)
- [API Reference — Tile](https://docs.tomorrow.io/reference/retrieve-a-tile-basic)
- [OpenAPI](openapi/tomorrow-io-map-tiles-api-openapi.yml)
- [Naftiko Capability — Map Tiles](capabilities/weather-map-tiles.yaml)

### Tomorrow.io Locations API
Manage saved locations (points, polygons, lines) referenced by `locationId` across the Tomorrow.io APIs, with tag-based cohorts for fleet, customer, or asset organization.

**Human URL:** [https://docs.tomorrow.io/reference/list-locations](https://docs.tomorrow.io/reference/list-locations)

- [API Reference](https://docs.tomorrow.io/reference/list-locations)
- [OpenAPI](openapi/tomorrow-io-locations-api-openapi.yml)
- [JSON Schema — Location](json-schema/tomorrow-io-location-schema.json)
- [Naftiko Capability — Locations](capabilities/locations.yaml)

### Tomorrow.io Alerts API
Create and manage threshold-based weather alerts that evaluate Tomorrow.io data layers against custom rules for linked locations and deliver notifications via webhook, email, and the Tomorrow.io app.

**Human URL:** [https://docs.tomorrow.io/reference/create-alerts](https://docs.tomorrow.io/reference/create-alerts)

- [API Reference](https://docs.tomorrow.io/reference/create-alerts)
- [OpenAPI](openapi/tomorrow-io-alerts-api-openapi.yml)
- [JSON Schema — Alert](json-schema/tomorrow-io-alert-schema.json)
- [Example — Alert](examples/tomorrow-io-alert-example.json)
- [Naftiko Capability — Alerts](capabilities/alerts.yaml)

### Tomorrow.io Insights API
Define and manage reusable Insights — named rules combining Tomorrow.io data layers, operators, and thresholds — that power the Events and Alerts APIs.

**Human URL:** [https://docs.tomorrow.io/reference/list-insights](https://docs.tomorrow.io/reference/list-insights)

- [API Reference](https://docs.tomorrow.io/reference/list-insights)
- [OpenAPI](openapi/tomorrow-io-insights-api-openapi.yml)
- [JSON Schema — Insight](json-schema/tomorrow-io-insight-schema.json)
- [Naftiko Capability — Insights](capabilities/insights.yaml)

## Features

- 60+ Hyperlocal Data Layers
- Proprietary Microsatellite Weather Radar Constellation
- Minutely Forecast Resolution (Enterprise)
- 14-Day Forecast Horizon
- Climate Normals
- Severe Weather and Custom Events
- Threshold Alerts with Webhooks
- Weather Map Tiles
- Weather on Routes
- Official MCP Server for Agentic AI
- 99.9% Uptime SLA (Enterprise)
- LLMs.txt Indexed Documentation

## Pricing and Rate Limits

| Tier | Calls/sec | Calls/hour | Calls/day | Forecast | Historical |
|---|---|---|---|---|---|
| Free | 3 | 25 | 500 | 5 days | 24 hours |
| Basic | quote | quote | quote | extended | extended |
| Professional | quote | quote | quote | extended | extended |
| Enterprise | quote | quote | quote | 14 days | full archive |

- [Plans](plans/tomorrow-io-plans-pricing.yml) — API Commons Plans 0.1
- [Rate Limits](rate-limits/tomorrow-io-rate-limits.yml) — API Commons Rate Limits 0.1
- [FinOps](finops/tomorrow-io-finops.yml) — FinOps Framework / FOCUS 1.3

Note: each requested field in a single API call counts as one call against the quota.

## Use Cases

Route optimization, aviation operations, energy forecasting, agriculture, severe-weather alerting, sports and outdoor events, insurance and climate risk, data science, maritime operations, and on-demand platforms.

## Integrations

Mapbox, MapLibre, Leaflet, Google Cloud Functions, Netlify Edge, Postman, Model Context Protocol (MCP), webhooks.

## Common Resources

- [Portal](https://www.tomorrow.io)
- [API Documentation](https://docs.tomorrow.io)
- [API Reference](https://docs.tomorrow.io/reference/welcome)
- [Getting Started](https://docs.tomorrow.io/reference/getting-started)
- [API Keys](https://app.tomorrow.io/development/keys)
- [Sign Up](https://app.tomorrow.io/signup)
- [Console](https://app.tomorrow.io/signin)
- [Recipes Sandbox](https://docs.tomorrow.io/recipes)
- [Rate Limiting & Tokens](https://docs.tomorrow.io/reference/rate-limiting)
- [Error Handling](https://docs.tomorrow.io/reference/error-handling)
- [Release Notes](https://docs.tomorrow.io/reference/release-notes)
- [LLMs.txt](https://docs.tomorrow.io/llms.txt)
- [MCP Server](https://docs.tomorrow.io/reference/tomorrow-io-mcp)
- [Pricing](https://www.tomorrow.io/pricing/)
- [Terms of Service](https://www.tomorrow.io/legal/tos/)
- [Privacy Policy](https://www.tomorrow.io/legal/privacy-policy/)
- [Help Center](https://support.tomorrow.io)
- [Blog](https://www.tomorrow.io/blog/)
- [GitHub Organization](https://github.com/Tomorrow-IO-API)
- [LinkedIn](https://www.linkedin.com/company/tomorrow-io)
- [Twitter](https://twitter.com/tomorrow_io)

## Cross-Cutting Artifacts

- [Spectral Rules](rules/tomorrow-io-rules.yml)
- [Vocabulary](vocabulary/tomorrow-io-vocabulary.yml)
- [JSON-LD Context](json-ld/tomorrow-io-context.jsonld)

## Maintainer

Kin Lane (kin@apievangelist.com) — [@kinlane](https://x.com/kinlane)
