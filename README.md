# NEON CITY RP

Three.js 3D prototype for a GTA-style neon city.

## Structure

- `index.html` — game client
- `models/human_male.glb` — humanoid character asset
- `models/ferrari.glb` — Ferrari 458 asset

## Controls

- WASD — movement / driving
- Shift — run
- Space — jump
- E — enter/exit Ferrari
- Mouse — camera

The game starts without waiting for remote assets. It first tries local GLB files in `models/`, then remote sources.

## Important

The binary GLB model files are not included yet because the current GitHub connection cannot retrieve/upload the required binary assets from the external model hosts. Add the two GLB files to `models/` when available.
