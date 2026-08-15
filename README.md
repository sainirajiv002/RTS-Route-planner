# RTS Day Plan Portal

Interactive prototype for RTS (return-to-seller) day planning at Bamnoli B Block:
Block-A / NDD OFD manifests, reverse-fleet zone → cluster → route planning on a real
map, and a live rider/vehicle dispatch sheet — built on real operational data.

**Live demo:** enable GitHub Pages on this repo (Settings → Pages → Deploy from branch →
`main` / root) and it'll be served at `https://<your-username>.github.io/<repo-name>/`.

## What's in here

- `index.html` — the entire app. Single self-contained file: real geocoded route data
  is embedded inline, map tiles load from OpenStreetMap, Leaflet and SheetJS load from
  CDN. No backend, no build step, no server-side code.

## Status

This is a working **prototype**, not the production system. It's wired to one specific
day's dataset (`Assignment_file.xlsx`). Data doesn't persist and there's no login —
each visitor sees the same fixed snapshot. See the companion Excel workbook
(`rts_route_logic.xlsx`) for the live, editable version of the same routing logic.

## Local testing

No install needed — just open `index.html` directly in a browser, or serve it locally:

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```
