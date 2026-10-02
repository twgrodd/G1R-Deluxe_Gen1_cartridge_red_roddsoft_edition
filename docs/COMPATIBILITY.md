# Compatibility

## Baseline

- Target game: **Pokemon Red**
- Platform: **Gen1Recomp / Mod API 2**
- Cartridge: **G1R Deluxe — Red / Roddsoft Edition**

## Initial audit of supplied v0.1 collection

All 13 supplied manifests use API 2. None declares a hard dependency or an explicit conflict.

### Interaction requiring configuration

**Quality of Life 1.2.7 ↔ HM Anywhere 1.2.0**

Both provide contextual overworld HM interactions. Quality of Life can activate CUT/STRENGTH/SURF from contextual input; HM Anywhere also provides configurable contextual A-button CUT/SURF/STRENGTH. Do not enable both implementations of the same contextual feature until combined behavior is tested. The preferred cartridge policy is to let HM Anywhere own HM execution and use Quality of Life for its non-overlapping visual/QoL features.

### Designed optional integrations

Reusable Machines declares Modern Bag, Moves Manager, and HM Anywhere as optional dependencies. Keep those relative priorities intact.

Modern Bag, Moves Manager, Move Learn Stats, and Pokedex Plus contain optional Modern UI integration. Modern UI itself is not in the supplied v0.1 set, so those integrations must remain optional.

### Engine/version notes

New Game Plus requires Gen1Recomp >=0.1.38. Move Learn Stats accepts dev builds or >=0.1.38. The other supplied manifests use broader pre-2.0 ranges.

### Link-play notes

Moves Manager and Trade Evolution Fix declare `affects_link=true`. Treat link-play behavior as needing explicit combined testing before calling the cartridge link-safe.

### Redistribution

The supplied Quality of Life ZIP contains no LICENSE file. It remains a local candidate until redistribution permission is confirmed. The other third-party packages audited here include MIT license files.

## Test gate before release

1. Import legal Pokemon Red base data.
2. Validate/lint every packaged mod with upstream modkit.
3. Boot with the complete enabled set in deterministic order.
4. Test Bag/TM/HM/move-learning flows together.
5. Test contextual CUT, SURF and STRENGTH with only one owner enabled.
6. Test Pokedex, party Moves page, battle Move Inspector and EXP display.
7. Complete a trade/link smoke test for mods declaring affects_link.
8. Exercise New Game Plus only after a normal post-League save is available.
