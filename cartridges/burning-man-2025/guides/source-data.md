# Burning Man 2025 Source Data

This cartridge is seeded from the local Totem Grid checkout at:

`totem-grid-darwin`

Regenerate with `TOTEM_GRID_DARWIN_ROOT=/path/to/totem-grid-darwin node scripts/generate_burning_man_2025_cartridge.mjs` when the source checkout is somewhere else.

## Included

- 40 CPNS point features from `CPNS.swift`
- 45 toilet pins from `ToiletPins.swift`
- 10 plaza polygons from `Plazas.geojson`
- 1 trash fence polygon from `TrashFence.swift`

## Layer Counts

- boundary-waypoints: 5
- civic-hubs: 17
- emergency-services: 9
- ice: 2
- landmarks: 3
- logistics: 4
- plazas: 10
- toilets: 45
- trash-fence: 1

## Excluded For Now

- `StreetLines.geojson`: 599 LineString street features. The current Way2Crew cartridge client renders point pins and polygon fills from venue GeoJSON; forcing lines through the pin schema would produce misleading center pins.
- `amplitude.geojson`: separate event data outside Black Rock City.
- `MockData.swift` and `scripts/pin-generator.py`: prototype users, messages, and sample pins rather than event source data.

## Missing Source Data

- Assignment tasks and shift slots.
- Named crew roster.
- Operational guides.

## Tiles

- Base map: extracted from `https://build.protomaps.com/20260521.pmtiles` with bbox `-119.235,40.763,-119.174,40.809` and max zoom 15.
