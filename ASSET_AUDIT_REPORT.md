# 3D Asset Audit Report

Last checked: 2026-11-01T11:23:54+00:00
Run mode: Scheduled/normal full scan
Canonical model folder: assets/models/

**Overall status: PASS — runtime asset set complete; planned/optional assets remain outstanding.**

## Summary

| Check | Result |
|---|---:|
| GLB files present in assets/models/ | 12 |
| Required by current app | 8 / 8 present |
| UNESCO/site model slots | 4 / 8 present; 4 planned/optional missing |
| Optional environment props | 0 / 2 present |
| Unregistered model files | 0 |
| GLB files outside canonical folder | 0 |
| Invalid GLB containers | 0 |
| Non-standard filenames | 0 |
| Model files above recommended 5.00 MiB | 7 |
| Non-GLB files inside model folder | 0 |

## Current inventory

| Path | Size | GLB validation | Manifest role | Code reference |
|---|---:|---|---|---|
| assets/models/african_hut.glb | 9.34 MiB | PASS · optimize | African hut environment prop | Yes |
| assets/models/artifact.glb | 4.48 MiB | PASS | Board-game artifact token | Yes |
| assets/models/beach_environment.glb | 1.91 MiB | PASS | Beach / coastal environment | Yes |
| assets/models/borobudur_temple.glb | 5.20 MiB | PASS · optimize | Borobudur Temple | Yes |
| assets/models/classical_statue.glb | 8.21 MiB | PASS · optimize | Classical statue | No |
| assets/models/egyptian_head.glb | 13.55 MiB | PASS · optimize | Egyptian head statue | No |
| assets/models/komodo_dragon.glb | 5.85 MiB | PASS · optimize | Komodo dragon | Yes |
| assets/models/komodo_island.glb | 14.22 MiB | PASS · optimize | Komodo island — Elin model | Yes |
| assets/models/prambanan_temple.glb | 846.9 KiB | PASS | Prambanan / Candi Siwa | Yes |
| assets/models/school_building.glb | 422.5 KiB | PASS | Low-poly school building | Yes |
| assets/models/statue_of_bastet.glb | 2.00 MiB | PASS | Statue of Bastet player token | Yes |
| assets/models/wounded_amazon_statue.glb | 10.77 MiB | PASS · optimize | Wounded Amazon statue | No |

## Runtime-required assets

| Final filename | Status | Used by |
|---|---|---|
| assets/models/borobudur_temple.glb | PRESENT | js/board.js, js/sites.js, data/sites.json |
| assets/models/artifact.glb | PRESENT | js/board.js |
| assets/models/statue_of_bastet.glb | PRESENT | js/board.js |
| assets/models/beach_environment.glb | PRESENT | js/board.js |
| assets/models/school_building.glb | PRESENT | js/board.js |
| assets/models/african_hut.glb | PRESENT | js/board.js |
| assets/models/prambanan_temple.glb | PRESENT | js/app.js, js/sites.js, data/sites.json |
| assets/models/komodo_dragon.glb | PRESENT | js/app.js, js/sites.js, data/sites.json |

## Missing planned / optional files

Upload each file to the exact path shown. Use a single .glb with embedded textures.

| Expected filename | Priority | Subject | Source / note |
|---|---|---|---|
| assets/models/bali_subak_landscape.glb | planned | Bali subak landscape | Source to be identified — To be confirmed |
| assets/models/sangiran_fossil_display.glb | planned | Sangiran fossil learning display | Source to be identified — To be confirmed |
| assets/models/lorentz_highland_forest.glb | planned | Lorentz highland forest | Source to be identified — To be confirmed |
| assets/models/borobudur_relief_3rd_floor.glb | optional | Borobudur relief detail | [Source](https://sketchfab.com/3d-models/borobudur-3rd-floor-relief-pictograph-2c49eeb628684757b8f0f87165a12007) — CC BY; verify current terms and attribution at source |
| assets/models/palm_tree.glb | optional | Palm tree prop | [Source](https://marina-sunny-girl.itch.io/free-modular-islands-pack) — CC0 (check exact source item) |
| assets/models/coastal_rock.glb | optional | Coastal rock prop | [Source](https://marina-sunny-girl.itch.io/free-modular-islands-pack) — CC0 (check exact source item) |

## Unsupported file formats in assets/models

- None


## New, changed and removed since previous audit

Compared with the previous asset audit baseline.

### New files

- assets/models/komodo_dragon.glb
- assets/models/komodo_island.glb
- assets/models/prambanan_temple.glb

### Changed file contents

- assets/models/borobudur_temple.glb

### Removed files

- None

## Findings and cleanup candidates

- No unregistered GLB is currently present in the canonical model folder.

### Present but not referenced in executable code

These files are retained rather than deleted automatically. Decide whether to reuse or remove them in a separate reviewed change.

- assets/models/classical_statue.glb — 8.21 MiB
- assets/models/egyptian_head.glb — 13.55 MiB
- assets/models/wounded_amazon_statue.glb — 10.77 MiB

### Optimisation warnings

Recommended maximum is 5.00 MiB. Large files may load slowly in GitHub Pages / browser gameplay.

- assets/models/african_hut.glb — 9.34 MiB
- assets/models/borobudur_temple.glb — 5.20 MiB
- assets/models/classical_statue.glb — 8.21 MiB
- assets/models/egyptian_head.glb — 13.55 MiB
- assets/models/komodo_dragon.glb — 5.85 MiB
- assets/models/komodo_island.glb — 14.22 MiB
- assets/models/wounded_amazon_statue.glb — 10.77 MiB

## What this audit does not do

- It only checks files already in the repository; it does not search for or download new 3D models.
- It cannot confirm copyright/licence permission, archaeological accuracy, topology quality, texture appearance or in-game scale.
- New files placed in assets/models/ are reported; register their purpose and licence in data/asset_manifest.json after review.

Full filename list and upload steps: ASSET_UPLOAD_GUIDE.md. Canonical metadata: data/asset_manifest.json.
