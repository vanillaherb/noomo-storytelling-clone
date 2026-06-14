# Noomo Storytelling Clone

Resource-level local clone of `https://storytelling.noomoagency.com/`.

## Setup

```powershell
python scripts\download_assets.py
python scripts\verify_static.py
python -m http.server 4173
```

Open `http://localhost:4173`.

## Notes

The site is a clean static reconstruction using public assets from the original page. It avoids shipping the original minified Nuxt bundle as the app implementation.

## Verification

- `python scripts\verify_static.py`
- Desktop smoke check at `http://localhost:4173`
- Mobile smoke check around 390x844

## Known Constraints

The clone uses public assets and a clean Three.js reconstruction. Some proprietary shader and exact Nuxt timeline behavior may be approximated when not directly exposed as reusable source.
