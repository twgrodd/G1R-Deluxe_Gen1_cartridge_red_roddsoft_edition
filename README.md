# G1R Deluxe — Gen 1 Cartridge: Red / Roddsoft Edition

Roddans dream-version of Pokemon Red.
Basically adding Quality of life improvements from newer games to the classic without removing the essence of the game.

## Status

**Current cartridge: v0.2.16** — sealed and release-ready, targeting Gen1Recomp `>=0.1.38`.

The cartridge uses a dark-red `#8b1624` shell, holo finish, and the custom Roddsoft label.

## Current mod lineup

1. Start Screen Roddsoft 1.0.2
2. Move Inspector 1.0.0
3. Running Shoes 1.10.0
4. Quality of Life 1.2.7
5. Move Learn Stats 1.0.2
6. Reusable Machines 1.0.1
7. Exp Share 0.1.10
8. New Game Plus 1.0.0
9. All Pokémon Catchable 151 Mod — Roddsoft-compatible fork 0.3.3
10. Trainer Rematch Roddsoft 0.5.4
11. Moves Manager 1.0.1
12. Modern Bag Roddsoft 1.6.6
13. Pokédex Plus 1.3.4
14. HM Anywhere 1.2.0
15. Crystal Animated Sprites with Shiny Visuals 2.0.3
16. Dramatic Shape 1.9.0

## Curated defaults

- **Running Shoes:** speed 1.5; FX off.
- **Quality of Life:** EXP bar on; location banners 2; Easy Interactions on; Water Interaction Surf First; Repel Prompt on; Pokédex Indicator ON (Gen2).
- **Exp Share:** Custom; Percent Slot All; Percent 10%; Single EXP Share All.
- **Modern Bag Roddsoft:** opening pocket last.
- **Dramatic Shape:** shiny odds 128; water off; battle back off; shadows off.

### Gen1Recomp display preferences

The intended display setup is **Voxel 0** and **TiltShift off**. These are Gen1Recomp engine/display settings and are not currently encoded in `cart.json` or the `.g1rcart`.

## Goals

- Target Pokémon Red explicitly.
- Combine compatible quality-of-life, graphics, gameplay, and content mods.
- Keep upstream mods attributable and versioned.
- Keep Roddsoft-specific compatibility changes isolated.
- Never distribute ROMs or ROM-derived assets.

## Cartridge format

This project is an official-style Gen1Recomp custom cartridge. The release artifact is a `.g1rcart` built from the root `cart.json` manifest. Published releases use strict validation and pinned GitHub mod releases.

See [CHANGELOG.md](CHANGELOG.md) for the complete version history.

## Upstream

Built for the Gen1Recomp mod platform:
https://github.com/bryanthaboi/gen1recomp

This repository is an independent fan project and is not affiliated with Nintendo, Game Freak, Creatures, or The Pokémon Company.

## Legal / content policy

Do not commit Pokémon Red ROM files, extracted proprietary assets, or ROM-derived bytes. Users must provide any required legally obtained game data themselves.
