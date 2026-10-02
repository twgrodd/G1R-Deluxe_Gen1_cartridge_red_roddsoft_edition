# Mod List

Authoritative inventory for the Roddsoft Edition cartridge. Versions below are from the ZIP archives supplied for the v0.1 collection.

| ID | Version | Category (manifest) | Priority | Status | Notes |
|---|---:|---|---:|---|---|
| move_inspector | 1.0.0 | QOL | 100 | candidate | No permissions requested |
| quality_of_life | 1.2.7 | UI | 100 | license review | ZIP contains no LICENSE; features default OFF |
| running_shoes | 1.4.1 | TWEAK | 100 | candidate | MIT; configurable movement extras |
| move_learn_stats | 1.0.2 | QUALITY_OF_LIFE | 120 | candidate | MIT; optional gen1_modern_ui |
| reusable_machines | 1.0.1 | QOL | 130 | candidate | MIT; integrates optionally with Modern Bag, Moves Manager, HM Anywhere |
| exp_share_modes | 1.0.0 | QOL | 140 | candidate | MIT |
| new_game_plus | 1.0.0 | QUEST | 320 | candidate | MIT; requires engine >=0.1.38 |
| trade_evolution_fix | 1.0.0 | GAMEPLAY | 500 | candidate | MIT; changes trade evolutions to level 40 |
| moves_manager | 1.0.1 | UI | 510 | candidate | MIT; affects_link=true; optional gen1_modern_ui |
| modern_bag | 1.6.0 | UI | 520 | candidate | MIT; optional gen1_modern_ui |
| pokedex_plus | 1.3.4 | UI | 540 | candidate | MIT; optional Modern UI 0.8.x/icon-fix integration |
| hm_anywhere | 1.2.0 | MECHANIC | 610 | candidate | MIT; contextual HM interactions configurable |
| startscreen_roddsoft | 1.0.1 | GRAPHICS | 100 | candidate | Red-only; Roddsoft original title ribbon |

## Intake notes

- All 13 manifests declare Mod API 2.
- No manifest declares a hard dependency or explicit conflict.
- The supplied Quality of Life archive has no LICENSE file, so it is not to be republished from this cartridge until redistribution permission is confirmed.
- Legacy/noncanonical category strings are preserved as supplied. Upstream validation may warn about them.
- Third-party source packages should remain unmodified where possible; cartridge-specific fixes belong in the integration layer.
