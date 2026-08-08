# Albie's Cyboard Imprint ZMK configuration

Custom firmware for the Cyboard Imprint, based on Cyboard Digital Tailor's
[ZMK user-config template](https://github.com/Cyboard-DigitalTailor/zmk-user-config-template).

## Upstream baseline

The configuration was migrated to Cyboard's July 2026 stable layout stack:

- ZMK `v0.3.0`
- Cyboard `zmk-keyboards` `v2026.07`
- `physical_layout_imprint_function_row_full_bottom_row`

These versions are deliberately pinned in `config/west.yml` so an upstream
layout change cannot silently shift key positions or break the thumb cluster.
The reusable GitHub Actions workflow is pinned to the matching ZMK release.

The left-half build enables [ZMK Studio](https://studio.cyboard.digital) over
USB. Hold the physical A- and F-position keys for three seconds to unlock it.
Studio changes are stored separately in keyboard flash; the keymap in this
repository remains the firmware default.

See Cyboard's
[current template documentation](https://github.com/Cyboard-DigitalTailor/zmk-user-config-template#readme)
before changing the pinned versions or physical layout.
