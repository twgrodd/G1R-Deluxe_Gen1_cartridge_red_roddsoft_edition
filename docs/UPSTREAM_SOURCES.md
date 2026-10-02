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

## Not found there

These supplied mods were not found in that repository at the audited versions:

- Running Shoes 1.4.1
- Quality of Life 1.2.7
- RoddSoft Edition Start Screen 1.0.1

The RoddSoft start-screen mod is our own project and already has its own
repository. It should be published as a proper versioned release before it is
pinned by the cartridge.

## Release-format blocker

At the time of this audit, `FAFF0x/gen1recomp` has no GitHub Releases. The
matched ZIPs are stored directly in the repository's `main` branch.

Gen1Recomp's official custom-cart tooling expects published GitHub or
GameBanana mod builds with immutable version/hash pins. A mutable branch file
must therefore not be treated as a final cartridge release pin.

Before `cart.json` is finalized, each included third-party mod needs a
cartkit-compatible published source (for example its canonical GitHub Release
or GameBanana build). If FAFF0x's branch-only ZIPs are the only distribution,
we need to determine the supported publication route rather than inventing a
release pin.
