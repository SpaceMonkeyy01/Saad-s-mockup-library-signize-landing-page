# Signize — Sign Mockup Studio

A lightweight landing page that catalogs a suite of photorealistic sign‑mockup
studios. Upload a logo, pick a sign type, and preview it on a wall. Each card
links out to its own hosted mockup app plus its source repository.

The whole page is a single, dependency‑free `index.html` — no build step, no
framework, no package manager.

## Live site

> Replace this with your Render URL after the first deploy, e.g.
> `https://signize.onrender.com`

## Features

- **Filter by category** — All types, Illuminated, Non‑Illuminated,
  Freestanding Signs, Building/Wall Signs.
- **Grid / List views** — toggle between a card grid and a compact list.
- **Per‑card links** — an "Open mockup studio" action and a GitHub source link.
- **Responsive** and keyboard‑accessible, with focus styles and ARIA states.

## Sign catalog

### Illuminated

| Sign | Type | Studio | Source |
|------|------|--------|--------|
| Face‑Lit Channel Letters | Illuminated Dimensional Letters | [Open](https://saad-s-face-lit-channel-letters-v1-0.ai.studio/) | [GitHub](https://github.com/SpaceMonkeyy01/Saad-s-Face-Lit-Channel-Letters-v1.0) |
| Halo‑Lit Channel Letters | Illuminated Dimensional Letters | [Open](https://saad-s-halo-lit-channel-letters-v1-0.ai.studio/) | [GitHub](https://github.com/SpaceMonkeyy01/Saad-s-Halo-Lit-Channel-Letters-v1.0) |
| Face & Halo‑Lit Channel Letters | Illuminated Dimensional Letters | [Open](https://face-halo-lit-channel-letters-v1-0.ai.studio/) | [GitHub](https://github.com/SpaceMonkeyy01/Saad-s-Face-Halo-Lit-Channel-Letters-v1.0) |
| Side‑Lit Channel Letters | Illuminated Dimensional Letters | [Open](https://saad-s-side-lit-channel-letters-v1-0.ai.studio/) | [GitHub](https://github.com/SpaceMonkeyy01/Saad-s-Side-Lit-Channel-Letters-v1.0) |
| Face & Side‑Lit Channel Letters | Illuminated Dimensional Letters | [Open](https://saad-s-face-side-lit-channel-letters-v1-0.ai.studio/) | [GitHub](https://github.com/SpaceMonkeyy01/Saad-s-Face-Side-Lit-Channel-Letters-v1.0) |
| Open Face Neon | Illuminated Dimensional Letters | [Open](https://saad-s-open-face-neon-v1-0.ai.studio/) | [GitHub](https://github.com/SpaceMonkeyy01/Saad-s-Open-Face-Neon-v1.0) |
| LED Neon | LED Neon Signs | [Open](https://saad-s-led-neon-v1-0.ai.studio/) | [GitHub](https://github.com/SpaceMonkeyy01/Saad-s-LED-Neon-v1.0) |
| LightBox Cabinet | Lightbox/Cabinet Signs | [Open](https://saad-s-lightbox-cabinet-v1-0.ai.studio/) | [GitHub](https://github.com/SpaceMonkeyy01/Saad-s-LightBox-Cabinet-v1.0) |
| Push‑Through Signage | Push‑Through Signage | [Open](https://saad-s-pushthrough-v1-0.ai.studio/) | [GitHub](https://github.com/SpaceMonkeyy01/Saad-s-PushThrough-v1.0) |

### Non‑Illuminated

| Sign | Type | Studio | Source |
|------|------|--------|--------|
| Fabricated Non‑Lit Letters | Dimensional Fabricated Letters | [Open](https://saad-s-fabricated-non-lit-letters-v1-0.ai.studio/) | [GitHub](https://github.com/SpaceMonkeyy01/Saad-s-Fabricated-Non-Lit-Letters-v1.0) |
| Flat Cut Letters | Dimensional Flat Cut Letters | [Open](https://saad-s-flat-cut-letters-v1-0.ai.studio/) | [GitHub](https://github.com/SpaceMonkeyy01/Saad-s-Flat-Cut-Letters-v1.0) |
| Wall Plaque | Wall Plaques | [Open](https://saad-s-wall-plaque-v1-0.ai.studio/) | [GitHub](https://github.com/SpaceMonkeyy01/Saad-s-Wall-Plaque-v1.0) |
| Wooden Sign | Wooden Signs | [Open](https://saad-s-wooden-sign-v1-0.ai.studio/) | [GitHub](https://github.com/SpaceMonkeyy01/Saad-s-Wooden-Sign) |

### Freestanding Signs

| Sign | Type | Studio | Source |
|------|------|--------|--------|
| Blade Projected Sign | Blade/Projecting Signs | [Open](https://saad-s-blade-projected-sign-v1-0.ai.studio/) | [GitHub](https://github.com/SpaceMonkeyy01/Saad-s-Blade-Projected-Sign-v1.0) |

### Building/Wall Signs

| Sign | Type | Studio | Source |
|------|------|--------|--------|
| Marquee Channel Letters | Marquee Signs | [Open](https://saad-s-marquee-channel-letters-v1-0.ai.studio/) | [GitHub](https://github.com/SpaceMonkeyy01/Saad-s-Marquee-Channel-Letters-v1.0) |

## Run locally

No tooling required — just open the file:

```bash
open index.html          # macOS
# or
xdg-open index.html      # Linux
```

Prefer a local server (handy for consistent relative paths)?

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy on Render

This repo ships a `render.yaml` Blueprint, so you have two options.

### Option A — Blueprint (recommended)

1. Push this repo (including `render.yaml`) to GitHub.
2. In the Render Dashboard choose **New > Blueprint** and select this repo.
3. Render reads `render.yaml` and creates the static site automatically. Click
   **Apply**.

### Option B — Manual static site

1. In the Render Dashboard choose **New > Static Site** and connect this repo.
2. Set the fields:
   - **Branch:** `main`
   - **Root Directory:** *(leave blank)*
   - **Build Command:** *(leave blank — nothing to build)*
   - **Publish Directory:** `.`
3. Click **Create Static Site**.

Either way, Render gives the site a unique `onrender.com` URL, serves it over a
global CDN, redirects HTTP to HTTPS, and redeploys automatically on every push
to the deployed branch. You can add a custom domain later from the dashboard.

## Project structure

```
.
├── index.html      # the entire site (markup, styles, and script inline)
├── render.yaml     # Render Blueprint (infrastructure as code)
└── README.md
```

## Author

Built by **Saad A.** ([@SpaceMonkeyy01](https://github.com/SpaceMonkeyy01)).
