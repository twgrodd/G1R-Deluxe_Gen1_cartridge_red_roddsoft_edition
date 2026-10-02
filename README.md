# G1R Deluxe — Gen 1 Cartridge: Red / Roddsoft Edition

A curated, ROM-free mod cartridge for Pokémon Red on the Gen1Recomp mod platform.

## Status

**v0.1 scaffold** — cartridge framework is in place; the curated mod set is the next milestone.

## Goals

- Target Pokémon Red explicitly.
- Combine compatible quality-of-life, graphics, audio, gameplay, and content mods.
- Keep upstream mods attributable and versioned.
- Keep Roddsoft-specific compatibility changes isolated.
- Never distribute ROMs or ROM-derived assets.

## Layout

- `cartridge/` — cartridge metadata and load order.
- `mods/` — curated/local mod content, grouped by purpose.
- `config/` — edition-level configuration.
- `patches/` — compatibility/integration patches only.
- `docs/MODLIST.md` — authoritative mod inventory.
- `docs/COMPATIBILITY.md` — conflicts and integration decisions.
- `docs/CREDITS.md` — upstream attribution.
- `docs/BUILDING.md` — setup/build notes.

## Upstream

Built for the Gen1Recomp mod platform:
https://github.com/bryanthaboi/gen1recomp

This repository is an independent fan project and is not affiliated with Nintendo, Game Freak, Creatures, or The Pokémon Company.

## Legal / content policy

Do not commit Pokémon Red ROM files, extracted proprietary assets, or ROM-derived bytes. Users must provide any required legally obtained game data themselves.

