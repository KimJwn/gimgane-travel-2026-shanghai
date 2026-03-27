# Developer Notes

## 2026-03-27 Shanghai Disney Map Alignment Baseline

### Final baseline accepted
- Sketch map background image offset is fixed to the right by `+40px`.
- Only the sketch background image is shifted; pins and roads stay unchanged.
- Castle is `CAST` (Fantasyland castle), not `GDN`.

### Centering rule
- Calibration map opens centered on saved `CAST` pin coordinates.
- Sketch map initial view centers on `CAST` position (`pos('CAST')`).
- `CAST` name is normalized to `캐슬(판타지랜드)`.
- `CAST` coordinates must not be force-reset to default if user moved them.

### Where to edit for future alignment tuning
- Sketch background x offset:
  - `maps/shanghai_disney_sketch_map.html`
  - `offline_pack/maps/shanghai_disney_sketch_map.html`
  - Search for `x:String(stretchedX+40)`.

### Safety note
- When adjusting visual alignment, move background first.
- Do not move route pins/roads unless user explicitly requests coordinate changes.
