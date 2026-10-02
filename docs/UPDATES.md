# Cartridge updates

Gen1Recomp supports update discovery for custom cartridges.

## User experience

An installed cartridge can be compared with the latest published cartridge release. When a newer compatible cartridge is available, the launcher can expose an **Update vX.Y.Z** action. The downloaded asset is a new `.g1rcart`, which is installed through the cartridge store.

This preserves the cartridge model: individual mods are pinned to exact builds rather than silently drifting to whatever their newest versions happen to be.

## Release procedure

1. Update and test the pinned mod set.
2. Bump `version` in the final root `cart.json`.
3. Commit the change.
4. Tag that commit `v<version>`, for example `v0.2.0`.
5. Push the tag.
6. GitHub Actions validates all pins online, packs `g1r-deluxe-red-roddsoft-<version>.g1rcart`, computes its SHA-256, and publishes both files to the GitHub Release.

The tag and `cart.json` version must match exactly.

## Why mod pins stay frozen

A released Roddsoft cartridge represents one tested combination. If an included mod publishes an update, that does **not** automatically mutate an existing cartridge release. We first test that mod version with the rest of the collection, update its pin/hash, bump the cartridge version, and publish a new cartridge.

That gives users a single cartridge-level update while preserving a reproducible known-good mod set.

## Current blocker

The repository intentionally does not yet contain the final root `cart.json`. Gen1Recomp's official cart schema requires published GitHub or GameBanana mod builds with exact hashes. The supplied local ZIP collection must first be mapped to legitimate published releases (or published where redistribution is permitted). Until then, the release workflow fails safely instead of publishing a non-reproducible cart.
