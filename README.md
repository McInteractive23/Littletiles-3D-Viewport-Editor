
A browser-based editor for [LittleTiles](https://github.com/CreativeMD/LittleTiles) selections. Paste in
exported SNBT, edit boxes individually or in groups, tweak corner offsets and face flips, preview the result
live in 3D, and export the edited selection back to SNBT.

Everything runs client-side — no build step, no server, no dependencies beyond Three.js loaded from a CDN.

**[Open the tool](https://YOUR-USERNAME.github.io/YOUR-REPO/)** · **[Read the guide](https://YOUR-USERNAME.github.io/YOUR-REPO/wiki.html)**

*(replace `YOUR-USERNAME`/`YOUR-REPO` above once this is pushed — see setup below)*

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
  index.html   — the tool itself (this is what GitHub Pages serves as the site root)
  wiki.html    — the guide/tutorial
README.md
```

## Setting up GitHub Pages

1. Push this repo to GitHub (create a new repo on GitHub, then from this folder:
   `git init`, `git add .`, `git commit -m "Initial commit"`,
   `git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO.git`, `git push -u origin main`).
2. On GitHub, go to **Settings → Pages**.
3. Under **Build and deployment → Source**, choose **Deploy from a branch**.
4. Set **Branch** to `main` and the folder to **`/docs`**, then **Save**.
5. GitHub will publish the site at `https://YOUR-USERNAME.github.io/YOUR-REPO/` within a minute or two —
   that URL loads `docs/index.html` directly, so visiting it drops you straight into the tool. The **📖 Guide**
   button in the tool's header links to `wiki.html`, and the guide links back to the tool.
6. Update the links at the top of this README once you know the real URL.

## Local use

No server needed — just open `docs/index.html` in a browser. Three.js and OrbitControls load from a CDN, so
you'll need an internet connection the first time (browsers cache the scripts after that).
