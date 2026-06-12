# MagnaCarto

Procedural cartography for personal knowledge graphs — your notes, rendered as a navigable medieval fantasy map.

**Phase 1 prototype.** Single file, no build step: open `index.html` in any browser.

## What it does

- ~150 sample PKM notes generated into 6 kingdoms (Philosophia, Vox, Fabula, Praxis, Aurum, Machina), each with provinces and notes-as-settlements
- Note prominence (links + recency) decides settlement size: city → town → hamlet
- Semantic zoom: **Grand Map** (kingdoms, terrain, sea creatures) → **Regional** (provinces, roads, major notes) → **Note View** (every note, hover for details)
- "Cartographer's Table" panel: label density / decoration / terrain detail sliders, plus toggles — the anti-clutter graphics settings
- Deterministic: same seed → same map. Change the seed and hit Redraw for a new world.

## Publish to GitHub Pages (one-time, ~3 minutes)

1. Create a new repo at <https://github.com/new> (e.g. `magnacarto`, public)
2. In this folder, run:
   ```
   git init
   git add .
   git commit -m "MagnaCarto Phase 1 prototype"
   git branch -M main
   git remote add origin https://github.com/<your-username>/magnacarto.git
   git push -u origin main
   ```
3. On GitHub: repo **Settings → Pages → Source: Deploy from a branch → main / (root)** → Save
4. After ~1 minute your map is live at `https://<your-username>.github.io/magnacarto/`

Every future `git push` updates the site automatically.

## Roadmap

- [ ] Real PKM imports (Tana, Obsidian, Roam, Notion, CSV…)
- [ ] Eterna theme + alternate visual themes
- [ ] Kingdom Selector UI (map categories → kingdoms)
- [ ] Hard/Soft generation modes with checkpoint versioning
- [ ] Publishing with privacy controls
