# Upstream mod sources

Release-candidate source audit for G1R Deluxe v0.1.0.

## FAFF0x/gen1recomp matches

The following supplied G1R Deluxe mods have an exact filename/version match in
`FAFF0x/gen1recomp` on its `main` branch:

| Mod | Version | Upstream file |
|---|---:|---|
| EXP Share Modes | 1.0.0 | `exp_share_modes_v1.0.0.zip` |
| HM Anywhere | 1.2.0 | `hm_anywhere_v1.2.0.zip` |
| Modern Bag | 1.6.0 | `modern_bag_v1.6.0.zip` |
| Move Inspector | 1.0.0 | `move_inspector_v1.0.0.zip` |
| Move Learn Stats | 1.0.2 | `move_learn_stats_v1.0.2.zip` |
| Moves Manager | 1.0.1 | `moves_manager_v1.0.1.zip` |
| New Game Plus | 1.0.0 | `new_game_plus_v1.0.0.zip` |
| Pokédex Plus | 1.3.4 | `pokedex_plus_v1.3.4.zip` |
| Reusable Machines | 1.0.1 | `reusable_machines_v1.0.1.zip` |
| Trade Evolution Fix | 1.0.0 | `trade_evolution_fix_v1.0.0.zip` |

Source repository:
https://github.com/FAFF0x/gen1recomp

## Quality of Life

Quality of Life 1.2.7 has a canonical GameBanana project:

- GameBanana mod ID: `699802`
- Page: https://gamebanana.com/mods/699802
- Cartridge source strategy: GameBanana pin rather than redistribution from this repository.

The final pin still needs the exact published file ID/build metadata and MD5
required by `cartkit`.

## Running Shoes

For v0.1.0, use Running Shoes **1.10.0**, replacing the older 1.4.1 candidate.

Canonical release:
https://github.com/MadeinTaly/gen1recomp-running-shoes/releases/tag/v1.10.0

Release asset:
`running_shoes-1.10.0.zip`

Verified SHA-256:
`d4a52154f9d6b9c81c2d7421b694beda79bd66ef45471d2b7064739a9f6ed37b`

The uploaded 1.10.0 archive matches the GitHub release asset digest exactly.
Its manifest identifies `running_shoes` version `1.10.0`, Mod API 2,
category `TWEAK`, priority 100, and GitHub source
`MadeinTaly/gen1recomp-running-shoes`.

## RoddSoft Start Screen

RoddSoft Edition Start Screen is original RoddSoft work and is now published
as a proper GitHub Release at **v1.0.2**.

Canonical release:
https://github.com/twgrodd/G1R-Deluxe_Gen1_mod_StartScreenRoddsoft/releases/tag/v1.0.2

Release asset:
`startscreen_roddsoft-1.0.2.zip`

Verified SHA-256:
`b8496d261312cef03baa167d647ab232391d9ff4dc2a4ea65a53c628f74445ec`

This replaces the earlier 1.0.1 cartridge candidate.

## Remaining release-format blocker

At the time of this audit, `FAFF0x/gen1recomp` has no GitHub Releases. Its
matched ZIPs are stored directly in the repository's `main` branch.

Gen1Recomp's official custom-cart tooling expects published GitHub or
GameBanana mod builds with immutable version/hash pins. A mutable branch file
must therefore not be treated as a final cartridge release pin.

Before `cart.json` is finalized, each included third-party mod needs a
cartkit-compatible published source. The ten FAFF0x-hosted mods therefore
still need their canonical release/GameBanana sources located, or another
supported immutable publication route confirmed.
