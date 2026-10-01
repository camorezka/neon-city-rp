# NEON CITY RP

Three.js 3D GTA-style neon city prototype.

## What is included

- `index.html` — complete browser game client.
- Procedural neon city with roads, buildings, lighting, fog and collision zones.
- Animated humanoid character loaded as GLB with Idle / Walk / Run / Jump state switching.
- Ferrari 458 GLB with driving, steering, wheel rotation and enter/exit interaction.
- Remote asset fallbacks so the game does not freeze waiting for one model host.
- Local asset fallbacks: `models/human_male.glb`, `models/ferrari.glb`.

## Controls

- **WASD** — walk / drive
- **Shift** — run
- **Space** — jump
- **E** — enter / exit Ferrari
- **Mouse** — third-person camera

## Assets

The current runtime uses the Quaternius-based humanoid build published by NafisRayan, which contains a character mesh, skeleton and 80+ named animation clips including Idle, Walk, Run and Jump. The source project documents the output as a single GLB ready for Three.js. citeturn1search0

The Ferrari uses the Three.js Ferrari GLB with a local-file fallback. The game starts immediately and loads the models independently, so a slow or unavailable asset host does not block the city.

For production/offline deployment, place the GLBs in `models/` and the client will use them as fallbacks.

## Deployment

The project is static and can be deployed directly to Vercel or GitHub Pages. No build step is required.
