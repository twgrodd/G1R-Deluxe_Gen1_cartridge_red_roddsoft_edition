# Changelog

This file records the evolution of **G1R Deluxe - Red / Roddsoft Edition** from the first cartridge release onward. It includes published releases as well as notable attempted versions that were not published.

## Starting point — v0.1.0 (2026-10-02)

The first official cartridge established the Roddsoft Edition as a **sealed Pokémon Red cartridge** for Gen1Recomp, requiring engine `>=0.1.38`, with a dark-red `#8b1624` shell, holo finish, and custom `label.png`.

The original 13-mod lineup was:

1. Start Screen Roddsoft 1.0.2
2. Move Inspector 1.0.0
3. Running Shoes 1.10.0
4. Quality of Life 1.2.7
5. Move Learn Stats 1.0.2
6. Reusable Machines 1.0.1
7. EXP Share Modes 1.0.0
8. New Game Plus 1.0.0
9. Trade Evolution Fix 1.0.0
10. Moves Manager 1.0.1
11. Modern Bag 1.6.0
12. Pokédex Plus 1.3.4
13. HM Anywhere 1.2.0

At this stage the cartridge pinned the mods and load order but did not yet define our later per-mod defaults.

## v0.1.1 (2026-10-02)

- Follow-up cartridge/label and release-workflow fix.
- Mod lineup and versions remained unchanged from v0.1.0.

## v0.2.0 (2026-10-03)

- Added the mod **Dramatic Shape 1.9.0**.
- Expanded the cartridge from 13 to 14 mods.

## v0.2.1 (2026-10-03)

Added the first curated per-mod default settings:

- Running Shoes: speed `1.5`, FX off.
- Quality of Life: EXP bar on, location banners `2`, Easy Interactions off.
- EXP Share Modes: Modern mode.
- Modern Bag: open the last-used pocket.
- Dramatic Shape: shiny odds `128`, water off, battle back off, shadows off.

## v0.2.2 (2026-10-03)

- Updated/upgraded the custom cartridge label presentation.

## v0.2.3 (attempted, not published)

- Attempted additional label compatibility work.
- The attempt did not produce a published GitHub release and was superseded by v0.2.4.

## v0.2.4 (2026-10-03)

- Reworked the cartridge build/release workflow to normalize the label during packaging for launcher compatibility.
- Build-time label handling converts the cartridge label to a 512×512 true-color RGB PNG.

## v0.2.5 (2026-10-03)

- Replaced the problematic label source with the clean user-supplied custom label.
- Kept the build-time normalization for launcher compatibility.

## v0.2.6 (2026-10-03)

- Added the mod **Crystal Animated Sprites with Shiny Visuals 2.1.0**.
- Expanded the cartridge to 15 mods.

## v0.2.7 (2026-10-04)

- Removed mod **Trade Evolution Fix 1.0.0**.
- Added mod **All Pokémon Catchable 151 Mod 0.3.3** from the original upstream repository.
- This gave the cartridge a broader all-151-without-trading solution, including replacements for the trade evolutions.
- The upstream release later proved unsuitable for a sealed cartridge because its internal manifest version did not exactly match the semver cartridge pin.

## v0.2.8 (attempted, not published)

- Tried to pin All Pokémon Catchable using its descriptive internal version string (`0.3.3-beta - Yellow Support Hotfix`) to match the upstream manifest.
- Gen1Recomp `cartkit` correctly rejected that value because cartridge mod versions must be valid semver.
- No v0.2.8 release was published.

## v0.2.9 (2026-10-04)

- Switched All Pokémon Catchable to the Roddsoft-compatible fork:
  `twgrodd/G1R-Deluxe_Gen1_mod_fork_All_Pokemon_Catchable`.
- Normalized the fork's internal manifest version to clean semver `0.3.3` while leaving gameplay code unchanged.
- Added a release workflow to the fork and pinned its validated v0.3.3 release.
- Resolved the sealed-cartridge version mismatch from v0.2.7.

## v0.2.10 (2026-10-05)

- Added mod **Trainer Rematch Roddsoft 0.5.4**.
- Switched mod **Modern Bag** from the original repository to the Roddsoft fork, initially pinned at v1.6.0.
- Repaired the unavailable mod Crystal Animated Sprites pin by moving from the vanished `notquiteog` repository/version 2.1.0 to the available `distilledorion-sketch` repository at v2.0.3.
- Strict online cartridge validation passed with the repaired release pins.

## v0.2.11 (2026-10-05)

- Updated the mod Roddsoft Modern Bag fork from v1.6.0 to **v1.6.4**.
- The fork's internal manifest was corrected to report v1.6.4 so the sealed cartridge and installed mod version agree.
- Preserved Modern Bag's `opening_pocket: last` default.

## v0.2.12 (2026-10-05)

- Removed mod **EXP Share Modes 1.0.0**.
- Added mod **Exp Share 0.1.10** (`ShaneMcGovernIE/exp_share`).
- The replacement provides OFF, Gen 1, Gen 5+, Balanced, Average, and Custom EXP-sharing modes plus single-slot and percentage controls.

## v0.2.13 (2026-10-05)

Configured the new Exp Share defaults:

- EXP Share: **Custom**
- Percent Slot: **All**
- Percent: **10%**
- Single EXP Share: **All**

Updated Quality of Life defaults:

- Easy Interactions: **On**
- Water Interaction: **Surf First**
- Repel Prompt: **On**

Existing QoL defaults such as the EXP bar and location banners were preserved.

## v0.2.14 (2026-10-05)

- Updated mod **Modern Bag Roddsoft 1.6.4 → 1.6.6**.
- Verified the v1.6.6 release's internal manifest also reports v1.6.6.
- Preserved the existing Modern Bag default settings.

## v0.2.15 (2026-10-06)

- Added Quality of Life default **Pokédex Indicator: ON (Gen2)**.
- This displays the Gen 2-style caught Poké Ball indicator during wild encounters for Pokémon already registered as owned.

## v0.2.16 (2026-10-06)

- Published a fresh cartridge build after revisiting the desired voxel presentation.
- Desired Gen1Recomp display setting changed from **Voxel 35** to **Voxel 0**.
- **Important:** Voxel is an engine/display setting, not a Dramatic Shape per-mod option exposed by the current official cartridge authoring schema. Therefore Voxel 0 is an intended external Gen1Recomp setting and is **not encoded in `cart.json` or the `.g1rcart`**.
- No gameplay mod pins or cartridge-encodable options changed from v0.2.15.

---

Release dates and published-version state above are based on the repository's GitHub release history. Entries for v0.2.3 and v0.2.8 are retained because they were meaningful development attempts even though they were not published releases.
