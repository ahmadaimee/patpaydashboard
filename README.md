# PatriotPay.ai — 3D Marketing Site

A single-page, cinematic marketing site for [PatriotPay.ai](https://patriotpay.ai), built with vanilla HTML/CSS/JavaScript and a real-time 3D galactic backdrop rendered with Three.js.

## Features

- **Real NASA Earth-from-ISS hero photo** that fades out on scroll into the cosmic 3D scene below.
- **Three.js scene** with a shader-driven black hole (Doppler-beamed accretion disk + gravitational lensing arcs), a Saturn-style banded gas giant with multi-band ring system (Cassini Division, Encke Gap), painted Andromeda-style spiral galaxy, supernova remnant, drifting nebula, comets, and a multi-layer photographic starfield with diffraction spikes on bright stars.
- **UnrealBloom post-processing** + ACES Filmic tone mapping for cinematic light.
- **Scroll-driven camera flight** through a 6-waypoint path past every phenomenon.
- **Glassmorphism UI** — frosted backdrop-filter blur on all cards, buttons, telemetry slab, and the demo-request form.
- **Cosmic trailing border** — animated conic-gradient comet trail orbiting every button and card.
- **PatriotPay brand palette** — graphite navy, gold (`#D4AF37`), blue (`#4A8FD4`), pale gold accent text.
- **HUD telemetry overlays** with live balance counter, sector readout, and chrono clock.

## Sections

1. **Hero** — "Patient Billing. Resolved." with telemetry stats
2. **The Singularity** — the strategy-problem manifesto
3. **The Platform** — four pillars (Predict / Engage / Assist / Resolve)
4. **Implementation** — 5-stage onboarding timeline
5. **Results** — real client case studies (Granite State Gastroenterology, New England Orthopedic, Mid-State Health Center)
6. **Begin** — demo request form

## Running

Open `index.html` in any modern browser (Chrome / Edge / Firefox / Safari). No build step, no dependencies, no install — Three.js is loaded from the unpkg CDN via an importmap.

For local development you'll want to serve over HTTP so the cubemap and texture loads aren't blocked:

```bash
npx serve .
# or
python -m http.server 8080
```

Then visit <http://localhost:8080>.

## Stack

- **Three.js 0.160** (CDN) — WebGL renderer, EffectComposer, UnrealBloomPass, OutputPass
- **Vanilla CSS** — custom properties, `@property` for animated conic gradients, `backdrop-filter` glassmorphism
- **Google Fonts** — Cormorant Garamond (display serif), Space Grotesk (sans), JetBrains Mono (UI)
- **Unsplash CDN** — hero Earth photograph
- **unpkg Three.js textures** — NASA Milky Way cubemap, lunar surface

## License

Code: MIT. Content (copy, brand) © PatriotPay.ai.
