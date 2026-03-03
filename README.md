# webxr-dev

A [Claude Code skill](https://skills.sh) for building WebXR/VR experiences with Three.js on Meta Quest.

## Install

```bash
npx skills add danielcanton/webxr-dev-skill
```

## What's Inside

Hard-won lessons from shipping VR on Meta Quest headsets:

- **Session setup** — `immersive-vr` vs `immersive-ar`, native framebuffer resolution, anti-pixelation
- **Camera rig architecture** — world-space vs local-space coordinates, `worldToLocal()` for rig children
- **Geometry rendering** — the `scale(-1,1,1)` + `BackSide` trap, why `DoubleSide` just works
- **Locomotion** — thumbstick mapping, ground-locked vs fly mode, smooth turn, vertical fly
- **Post-processing in VR** — `postprocessing` library has zero XR support; 3D alternatives for bloom, distortion, shockwaves
- **Object scale** — things that look fine on desktop feel enormous in VR
- **VR UI panels** — canvas-textured planes, raycasting, controller/hand interaction
- **Testing & debugging** — remote Chrome DevTools via `chrome://inspect`, Quest Developer Mode setup
- **11 common pitfalls** with fixes

## Usage

Once installed, invoke with `/webxr-dev` in Claude Code when adding VR support, debugging XR rendering, or implementing VR interactions.

## License

MIT
