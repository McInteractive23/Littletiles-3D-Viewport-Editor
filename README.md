
A browser-based editor for [LittleTiles](https://github.com/CreativeMD/LittleTiles) selections. Paste in
exported SNBT, edit boxes individually or in groups, tweak corner offsets and face flips, preview the result
live in 3D, and export the edited selection back to SNBT.

Everything runs client-side — no build step, no server, no dependencies beyond Three.js loaded from a CDN.

**[Open the tool](https://mcinteractive23.github.io/Littletiles-3D-Viewport-Editor/)** · **[Read the guide](https://mcinteractive23.github.io/Littletiles-3D-Viewport-Editor/wiki.html)**

## Features

- Import/export LittleTiles SNBT selections
- Per-box editing: position, size, block ID, color, alpha
- Bulk edit by texture group or color group
- Corner-offset and face-flip editing, with correct bit-packed encoding
- Live 3D preview (Solid / Solid+Wire / Wireframe view modes)
- Grid-aware floor reference, with presets up to 1024 and custom values above that

## Repo layout

```
docs/
  index.html   — the tool itself
  wiki.html    — the guide/tutorial
README.md
```

## Local use

No server needed — just open `docs/index.html` in a browser. Three.js and OrbitControls load from a CDN, so
you'll need an internet connection the first time (browsers cache the scripts after that).
