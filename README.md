<div align="center">

<img src="./assets/banner.svg" alt="Caelum — Beyond Every Horizon" width="100%" />

<br/>

<h1>✦ CAELUM</h1>

<p><strong>Beyond Every Horizon.</strong><br/>
An immersive, scroll-driven space-exploration landing page — from Earth departure to the Galilean moons.</p>

<p>
  <img alt="Status" src="https://img.shields.io/badge/status-prototype-F0B25A?style=flat-square" />
  <img alt="Three.js" src="https://img.shields.io/badge/Three.js-r128-F0B25A?style=flat-square&logo=three.js&logoColor=white" />
  <img alt="GSAP" src="https://img.shields.io/badge/GSAP-3.12.5-88CE02?style=flat-square&logo=greensock&logoColor=white" />
  <img alt="Lenis" src="https://img.shields.io/badge/Lenis-1.1.14-F0B25A?style=flat-square" />
  <img alt="Static" src="https://img.shields.io/badge/build-none%20·%20static-0A0A0C?style=flat-square" />
  <img alt="Deploy" src="https://img.shields.io/badge/deploy-Vercel-000000?style=flat-square&logo=vercel&logoColor=white" />
  <a href="https://www.kryoncode.xyz"><img alt="Made by KryptonCode" src="https://img.shields.io/badge/made%20by-KryptonCode-F0B25A?style=flat-square" /></a>
</p>

</div>

---

## ✦ Overview

**Caelum** is a fictional deep-space exploration company — *"We build the vessels, stations and signal networks that carry humanity past the edge of the map, and bring it back."*

This repository holds the **landing-page prototype**: a single, self-contained page that plays like a cinematic mission briefing. A live WebGL starfield and a slowly turning Earth sit behind buttery smooth-scroll, and every section is choreographed with motion — a launch countdown, a fleet reveal, a draggable orbit, and a signal-network map stretching to the Galilean moons.

It is a **design + front-end craft piece**: no framework app, no build step — just a hand-tuned document that runs straight in the browser.

---

## ✦ Features

- 🌍 **Live WebGL scene** — a depth-parallaxed starfield and a rotating Earth rendered with **Three.js**.
- 🪐 **Draggable orbit** — *"drag to take the helm"* — an interactive orbital system you can throw and let settle.
- 🛰️ **Signal-network map** — five installations holding the lattice open, from the ground to the Galilean moons.
- ⏱️ **Live launch countdown** — a real ticking `T–` clock to the next window (VELA-9 · Europa Relay · LC-39A).
- 🎞️ **Scroll choreography** — headlines, cards and telemetry reveal in sequence via **GSAP + ScrollTrigger**.
- 🧭 **Buttery smooth scroll** — inertial scrolling powered by **Lenis**.
- 🧲 **Magnetic buttons, 3D tilt cards, custom cursor glow** — tactile micro-interactions throughout.
- 🎛️ **Living background** — animated nebulae, a drifting telemetry grid, and switchable accents.
- 📱 **Responsive & glassmorphic** — a floating blurred nav and fluid `clamp()`-based type from phone to widescreen.

---

## ✦ The Journey

The page is one continuous flight, told across nine screens:

| # | Section | Beat |
|---|---------|------|
| `01` | **Hero** | *Beyond Every Horizon* — live launch countdown & GO-FOR-LAUNCH telemetry |
| `02` | **Mission** | *Engineered twice over — once for the void, once for the people inside* |
| `03` | **Systems** | The engineering backbone that makes departure possible |
| `—` | **Film** | An invitation to *watch the film* |
| `◦` | **Observatory / Orbit** | *Drag to take the helm* — the interactive orbital system |
| `04` | **Fleet** | *Built to leave* — the vessels of the program |
| `05` | **Network** | *One signal* — five installations to the Galilean moons |
| `06` | **Record** | The mission record and milestones |
| `07` | **Crew** | *Forty thousand engineers, pilots, students and stubborn optimists* |
| `08` | **CTA** | *Join* the Earth Departure Program |
| `09` | **Footer** | Sign-off and links |

---

## ✦ Tech Stack

| Layer | Tooling |
|-------|---------|
| **3D / WebGL** | [Three.js](https://threejs.org/) `r128` — starfield, Earth & orbital scene |
| **Animation** | [GSAP](https://gsap.com/) `3.12.5` + **ScrollTrigger** — scroll-linked motion |
| **Smooth scroll** | [Lenis](https://github.com/darkroomengineering/lenis) `1.1.14` |
| **Type** | [Clash Display](https://www.fontshare.com/fonts/clash-display) + [Satoshi](https://www.fontshare.com/fonts/satoshi) (Fontshare) · [IBM Plex Mono](https://fonts.google.com/specimen/IBM+Plex+Mono) |
| **Runtime** | `support.js` — a lightweight document runtime that auto-loads React 18 (UMD) from CDN and hydrates the page |
| **Build** | None. Static HTML + CDN libraries. |

---

## ✦ Design System

A dark, mission-control palette — a near-black void, a warm gold signal accent, and Earth-blue atmosphere.

| Swatch | Token | Hex | Role |
|:------:|-------|-----|------|
| ![](https://placehold.co/22x22/050505/050505.png) | Void | `#050505` | Page canvas |
| ![](https://placehold.co/22x22/EDEDF0/EDEDF0.png) | Ink | `#EDEDF0` | Primary text |
| ![](https://placehold.co/22x22/F0B25A/F0B25A.png) | Accent | `#F0B25A` | Signal · links · glow *(default)* |
| ![](https://placehold.co/22x22/4C86FF/4C86FF.png) | Earth | `#4C86FF` | Atmosphere / globe |
| ![](https://placehold.co/22x22/A5A5AF/A5A5AF.png) | Dim | `#A5A5AF` | Supporting copy |
| ![](https://placehold.co/22x22/6C6C76/6C6C76.png) | Faint | `#6C6C76` | Telemetry / labels |

The accent is themeable — the runtime also ships blue `#5B7CFF`, violet `#9D7BFF` and cyan `#38E1FF` as alternates.

**Type:** Clash Display for display headlines · Satoshi for body · IBM Plex Mono for eyebrows, labels and telemetry.

---

## ✦ Getting Started

No install, no build. Clone and open.

```bash
git clone https://github.com/ryhnxyz/caelum-space.git
cd caelum-space
```

**Quickest** — open the entry file directly in a modern browser:

```bash
open index.html      # macOS
xdg-open index.html  # Linux
start index.html     # Windows
```

**Recommended** — serve the folder (a couple of interactions behave best over `http://`):

```bash
npx serve .
# then open the printed http://localhost:… URL
```

> **Note** — keep `support.js` next to `index.html`; the page loads it relatively. Three.js, GSAP, Lenis and React load from CDN, so an internet connection is needed on first paint.

---

## ✦ Deploy

The site is fully static with `index.html` at the repo root, so it hosts anywhere with **zero configuration**.

**Vercel** — import the repo and deploy. No build step needed:

| Setting | Value |
|---------|-------|
| Framework Preset | **Other** |
| Build Command | *(leave empty)* |
| Output Directory | *(leave empty / repo root)* |

The entry `index.html` is served at `/` automatically. Works the same on **Netlify**, **Cloudflare Pages**, or **GitHub Pages**.

---

## ✦ Project Structure

```text
caelum-space/
├─ index.html      # the landing page (design-canvas export) — site entry point
├─ support.js      # dc-runtime: auto-loads React from CDN, hydrates the page
├─ assets/
│  └─ banner.svg   # the hero banner in this README
└─ README.md
```

---

## ✦ Roadmap

- [ ] Publish the live URL in this README
- [ ] Self-host fonts & libraries for full offline / no-CDN loading
- [ ] A `prefers-reduced-motion` low-motion mode
- [ ] Lighthouse & performance pass

---

## ✦ Credits

Designed & built by **[KryptonCode](https://www.kryoncode.xyz)**.

<div align="center">
<br/>

**✦ CAELUM** — *Beyond Every Horizon*

[![Visit KryptonCode](https://img.shields.io/badge/www.kryoncode.xyz-F0B25A?style=for-the-badge&logoColor=black)](https://www.kryoncode.xyz)

<sub>Crafted by KryptonCode · www.kryoncode.xyz</sub>

</div>
