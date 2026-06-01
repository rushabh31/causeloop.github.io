# Causeloop — Marketing Site

> **Find the cause, break the loop.**
> AI-native risk intelligence that connects fragmented issue data into the thematic
> patterns behind recurring failures, predicts where risk appears next, and recommends
> what to do about it.

This repository contains the production marketing website for **Causeloop**, deployed
via GitHub Pages.

## ✦ Highlights

- **Single-page, zero-dependency** site — pure HTML, CSS and vanilla JS. No build step.
- **Light & dark mode** — respects the visitor's system preference and remembers their
  choice (`localStorage`). Toggle in the nav.
- **Fully responsive** — fluid type and layout from 320px phones to wide desktops.
- **Accessible** — skip link, semantic landmarks, keyboard-friendly nav, visible focus
  states, and full `prefers-reduced-motion` support.
- **Performance-minded** — system + Google fonts with `preconnect`, IntersectionObserver
  reveals, no heavy frameworks.

## 🎨 Brand system

Sourced directly from the Causeloop brand guidelines.

| Token | Hex | Role |
| --- | --- | --- |
| Deep Navy | `#1E2A5A` | Primary · wordmark |
| Terracotta | `#E2603F` | Accent · "the cause" |
| Slate | `#5A6480` | Body text |
| Paper | `#FBFBFC` | Canvas |

**The mark** is a loop that nearly closes — the recurring cycle of risk — then *breaks
outward into an arrow*: the cycle escaped. It carries the brand **blue gradient**
(cobalt `#4A78FF` → cyan `#1FC2FF`), and a single terracotta point marks the **root
cause** the platform surfaces.

### The "Loopface" type system

The brand voice is carried by a unified, three-weight type system tuned with bespoke
optical tracking so it reads as one signature typeface family:

- **Display / wordmark** — Schibsted Grotesk (800–900), tight `-.05em` tracking.
- **Text** — Hanken Grotesk.
- **Signal / mono** — JetBrains Mono (labels, metrics, eyebrows).

## 📁 Structure

```
.
├── index.html              # the site
├── assets/
│   ├── css/style.css       # design tokens, themes, layout
│   ├── js/main.js          # theme toggle, reveals, count-up, nav, form
│   └── img/
│       ├── favicon.svg     # app mark
│       └── og-image.svg    # social share card
├── .nojekyll               # serve assets/ untouched by Jekyll
├── robots.txt
└── sitemap.xml
```

## 🚀 Local preview

No tooling required — open `index.html`, or serve the folder:

```bash
python3 -m http.server 8000
# → http://localhost:8000
```

## 📦 Deployment

Hosted on **GitHub Pages**. Pushing to the default branch publishes the site.
Settings → Pages → *Deploy from a branch* → root.

---

© Causeloop. Find the cause · break the loop.
