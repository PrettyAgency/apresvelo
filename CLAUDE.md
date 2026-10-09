# Après Vélo — project notes

- Seven pages, all at project root: `Index.dc.html`, `V1 Tasmania Hub.dc.html`, `V1 Tour de Tasmania.dc.html`, `V2 Tasmania Hub.dc.html`, `V2 Tour de Tasmania.dc.html`, `V3 Tasmania Hub.dc.html`, `V3 Tour de Tasmania.dc.html`.
- V1 pages are FROZEN (21 Sep 2026). V2 pages are FROZEN as of 9 Oct 2026. Do not edit.
- All ongoing work happens in the V3 pages. Default to editing V3 unless the user explicitly says otherwise.
- `Index.dc.html` is the client start page linking all versions.

## V3 colour change log (9 Oct 2026) — to undo, reverse these find/replaces in V3 Tasmania Hub, V3 Tour de Tasmania and route-map.html
Applied as global literal replacements (new → original):
- #ffffff → #f2efe8 (oat; page bg AND cream text/borders on dark sections)
- #f3f4f5 → #faf8f3 (milky white / light panels)
- #e8eaec → #e6e1d4 (darker oat panels)
- #dfe2e5 → #ddd8cc (borders)
- rgba(255,255,255 → rgba(242,239,232 (translucent cream overlays)
- route-map.html tile filter: grayscale(1) brightness(1.08) contrast(0.92) → grayscale(1) sepia(0.35) brightness(1.06) contrast(0.9)
Caution: if any genuinely-white (#ffffff) elements were added to V3 after this date, they'd also revert — V2 files hold the original palette for reference (V2 is identical to pre-change V3 apart from later edits).
Forest green #1f3d33 and red #cf0a2c unchanged (client-approved).
