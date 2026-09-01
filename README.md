# Aegivault

Aegivault is a mobile-first emergency coordination simulator for training, product demonstration, and interface prototyping. It is not certified for live emergency response and must not be used as an operational dispatch system.

## MVP experience

The app includes a command overview with system status and a live field map, active incident triage with severity filters, incident detail with priority assessment and timeline, simulated dispatch recommendations, unit readiness and availability, GIS-style map view with incidents/responders/facilities, hospitals and safe-route actions, communications and system-control modules, and an always-visible simulation-mode indicator.

The app is designed as an installable, app-like experience with a compact mobile navigation model. On wider screens the same interface expands into a centered operations canvas with a vertical navigation rail.

## Run locally

```bash
pnpm install
pnpm dev
```

## Build and serve

```bash
pnpm build
pnpm start
```

## Source map

- `client/src/App.jsx` contains the JavaScript app shell, incident data, views, simulation interactions, and navigation.
- `client/src/index.css` contains the Aegivault visual system and responsive layout.
- `client/public/manifest.json` contains installable app metadata.
- `client/public/favicon.svg` contains the Aegivault mark.
- `server/index.js` serves the compiled static app.

## Visual system

Aegivault uses a dark graphite operations field with cyan for navigation and GIS structure, signal yellow for active attention and command actions, rescue red for critical incidents, and safety green for availability and confirmed states. Typography pairs Manrope with DM Mono for operational labels, IDs, and telemetry-style values.

## Future integration points

The demo data in `client/src/App.jsx` should be replaced with server-authoritative incident, unit, hospital, identity, and event-stream APIs. A production system would require rigorous authentication, authorization, audit logging, secure communications, reliable geospatial services, observability, accessibility validation, and formal emergency-services certification before operational use.
