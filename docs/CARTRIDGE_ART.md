# Cartridge appearance

Gen1Recomp custom carts expose launcher appearance through the official cart schema.

## Roddsoft Edition visual spec

- Shell: `#8b1624` — deep cartridge red
- Finish: `holo`
- Base: `red`
- Label filename: `label.png`
- Working label canvas: **96 × 96 PNG**
- Cart title: **G1R Deluxe - Roddsoft Edition**

The launcher maps the label PNG into the cartridge's recessed label surface and applies the selected finish effect.

## Supported appearance fields

`shell` accepts a six-digit RGB hex color.

`finish` accepts `sparkle`, `holo`, or `sparkle+holo`.

`label` is a relative PNG path inside the cart bundle. Gen1Recomp's cartkit scaffold creates a 96 × 96 PNG; custom PNG dimensions are accepted by the renderer, but square artwork is the safest authoring target for the GB-style shell.

## Important

`cartridge/cart.visual.json` is a visual/schema draft, not the final packable `cart.json`.

The official cart format requires every included mod to be pinned to a published GitHub or GameBanana build with the expected release hash. Once the supplied mod ZIPs have legitimate published sources/releases, promote this visual configuration into the final `cart.json` and pin the complete mod set.
