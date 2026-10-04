# Skyline Series — Generative Art

> A seed-based generative system for themed cityscapes.  
> A reproducible catalogue of computational textile compositions.

---

## What is this?

**Skyline Series** is a generative design system that renders eight themed cities from a single numeric seed. A seed picks one of eight palettes — Pinky Dream, Toxic Neon Green, Cool Blue Night, Inferno Red, Mystic Purple, Golden Gothic Dusk, Cyber Cyan, Emerald Moon — then lays a field of buildings across the canvas, each with its own palette, its own sky tint, and its own window logic.

Every artwork in this catalogue is defined by a single numeric seed. The same seed always produces the identical composition — making each piece **traceable, reproducible, and licensable** across textile, print, and apparel applications.

Named for the line a city draws against its sky — the horizontal rhythm that repeats across every rooftop — **Skyline Series** translates that logic into code.

---

## Live

🌐 **[View the catalogue →](https://reyrove.github.io/Skyline-Series-Generative-Art/)**

---

## The System

The generator combines three layers:

| Layer | Description |
|-------|-------------|
| **Buildings** | 6–11 sheared rectangles, each with gridded facades, randomised width and height, and a theme-driven spire probability. |
| **Windows** | Lit cells drawn inside each facade — in checker, stripe, diamond, or random arrangement, chosen per theme. |
| **Sky** | A scatter of stars and outline shapes — triangles, diamonds, polygons — tinted by the theme's sky overlay. |

All three layers are driven by the same seed, ensuring deterministic output.

### Parameters

- **Theme** — one of eight curated city palettes, chosen per seed
- **Building count** — 6 to 11 per composition
- **Facade lines** — vertical and horizontal, theme-driven density
- **Window pattern** — checker / stripes / diamond / random
- **Spire probability** — 0.3 to 0.8, set by theme
- **Stars** — 18 to 32, scattered across the upper canvas
- **Sky shapes** — 18 outline forms per composition

---

## Structure

```
Skyline-Series-Generative-Art/
├── index.html          ← Full catalogue (single-file)
├── images/
│   ├── fav.svg
│   ├── tote.png
│   ├── tee.png
│   └── cushion.png
└── README.md
```

The entire project is contained in a single `index.html` — no build step, no framework. Open it in any modern browser.

---

## Features

- **Seed-based generation** — every composition is deterministic and reproducible
- **Eight themed cities** — each with its own palette, sky tint, and window logic
- **Live catalogue** — cover, plate, surfaces, process, archive, commission sections
- **Multiple surfaces** — print, scarf, textile, wallpaper — all rendered from the same seed
- **Archive of 8 seeds** — click any plate to load it into the main view
- **PNG export** — download any composition directly from the browser
- **Keyboard shortcuts** — `R` for new seed, `S` to save
- **Legal modal** — licensing, terms, and credits built in
- **Responsive** — works on desktop, tablet, and mobile
- **Mobile-first navbar** — horizontally scrollable with fade hint

---

## Usage

### Generate a new composition

Click **New Seed** or press `R`.

### Download the current composition

Click **Download** or press `S`.

### Load a seed from the archive

Click any plate in the **Archive** section.

---

## Colour System

Each seed selects one of eight themed cities:

| Theme | Character |
|-------|-----------|
| **Pinky Dream City** | Rose, blush, deep plum — checker windows |
| **Toxic Neon Green City** | Acid green, deep moss — random windows |
| **Cool Blue Night** | Steel, ice, midnight — stripe windows |
| **Inferno Red City** | Ember, rust, amber — chaotic windows |
| **Mystic Purple Realm** | Violet, lilac, deep indigo — diamond windows |
| **Golden Gothic Dusk** | Ochre, brass, warm bronze — checker windows |
| **Cyber Cyan City** | Electric cyan, deep teal — stripe windows |
| **Emerald Moon Night** | Jade, sage, cool green — random windows |

Each theme carries a full palette — a background, a set of building colours, a set of window colours, a sky overlay tint, and a config object that governs spire probability, facade line density, and window pattern.

---

## Technical Notes

- p5.js 1.9.0 (CDN) for canvas rendering
- Custom seeded random generator for deterministic output
- RGB colour mode, per-instance
- Buildings drawn with `shearX()` for a slight architectural lean
- Windows drawn as a grid within each facade rectangle
- Rectangular surfaces tile the square composition to fill aspect ratio

---

## About

**Skyline Series** is a project by [Reyhaneh Daneshdoost](https://reyrove.github.io/) — an Iranian-born artist working at the intersection of classical textile logic and generative systems.

The work begins with a simple observation: the woven surface — repetitive, mathematically structured, infinitely variable — has always been a form of computation, long before computers.

**Skyline Series** is an attempt to render that logic visible.

> *Eight cities, one seed — a skyline is a grid seen from the side.*

---

## Licensing

All compositions are seed-documented and available for licensing across textile, surface, and apparel applications.

For commercial use, custom editions, or exclusive rights:

📧 **reyhanehdaneshdoost@gmail.com**

See the **Licensing** section in the live catalogue for details.

---

## Links

- 🌐 [Website](https://reyrove.github.io/)
- 📷 [Instagram](https://www.instagram.com/rey._.rove/)
- 💼 [LinkedIn](https://www.linkedin.com/in/reyhaneh-daneshdoost-730481160/)
- 🐦 [X](https://x.com/reyrove)

---

## Credits

**Design & Generative System**  
Reyhaneh Daneshdoost

**Typefaces**  
Cormorant Garamond · DM Mono

**Edition**  
Skyline Series — Autumn 2026

---

<p align="center">
  <em>Computational Textile Design</em><br />
  <sub>© Reyrove Studio · All compositions reproducible by seed</sub>
</p>