# Building / Testing

The cartridge is currently a v0.1 scaffold.

## Requirements

1. Obtain and set up Gen1Recomp from its upstream project.
2. Follow Gen1Recomp's instructions to import your own legally obtained Pokémon Red game data.
3. Do not place ROM files or extracted proprietary assets in this repository.
4. Add curated mods according to `docs/MODLIST.md`.
5. Apply the cartridge load order from `cartridge/loadorder.lua`.

## Validation target

As the mod collection is populated, validation should use Gen1Recomp's modkit against imported base data where applicable:

```sh
python3 tools/modkit.py validate mods/<mod-id> --base imported
python3 tools/modkit.py lint mods/<mod-id>
```

Each included/local mod should eventually have an effect-level test, not merely a load test.
