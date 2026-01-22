# Felt Spatial Analyst

A browser-based spatial analysis tool for [Felt](https://felt.com) maps, powered by [Turf.js](https://turfjs.org/).

## Live Demo
**https://makella.github.io/felt-spatial-analyst/**

## Features

### Spatial Analysis Tools
- **Buffer Analysis** — Draw a buffer around a point and count features inside
- **Nearest Neighbor** — Find the N closest features to any location
- **Layer Statistics** — Get summary stats: feature count, total area, length, attribute breakdown
- **Point-in-Polygon Query** — Click to find which polygon contains a point

### Core Features (inherited from Felt Explorer)
- Load any Felt map by URL
- Real-time viewport tracking
- Layer visibility toggle
- Feature inspection
- Recent maps saved locally

## How It Works

1. **Paste a Felt map URL** to load any public map
2. **Select a layer** from the Analysis dropdown
3. **Choose a tool** (Buffer, Nearest, Stats, or Point Query)
4. **Pan the map** to position the crosshair at your analysis point
5. **Click Run** to execute the analysis

## Tech Stack

- [Felt JS SDK](https://feltmaps.github.io/js-sdk/) — Map embedding & interaction
- [Turf.js](https://turfjs.org/) — Spatial analysis operations
- Vanilla JavaScript — No build step required
- GitHub Pages — Static hosting

## Limitations

- Client-side only (no server) — works best with <10k features
- Analysis uses map center as reference point (no direct click capture)
- Some Felt layers may not expose features via SDK

## Related

- [Felt Explorer](https://makella.github.io/felt-explorer/) — The base map explorer app
- [Felt Documentation](https://feltmaps.github.io/js-sdk/)
