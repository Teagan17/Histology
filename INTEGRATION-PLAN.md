# Histology website integration plan

This branch is the polished interface working copy. Keep the interface independent until it is stable.

## Renal / urinary

The renal/urinary collection includes a dedicated **Ureter** entry. This is intentionally integration-ready: the ureter slide can later be connected to the professor's Virtual Slide Box stack/manifest without redesigning the collection page.

## Integration order

1. Finish and test the Histology interface.
2. Keep the professor's viewer and manifests as the source of truth for high-resolution scans.
3. Map each educational slide to a viewer/stack identifier.
4. Replace the ureter placeholder with the actual ureter viewer connection.
5. Reuse the same viewer connection pattern for kidney, bladder, and additional tissues as scans become available.

Do not copy large virtual-slide scan files into the Histology `images/` folder. The final combined application should use the professor's viewer infrastructure for those scans.
