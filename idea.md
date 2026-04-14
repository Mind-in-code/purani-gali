# PURANI GALI — Crafted Attar Brand Website

## Project Overview
A luxury website for **Purani Gali**, a crafted attar (oil-based perfume) brand. Dark, elegant, premium aesthetic with 3D interactive elements. Uses a blend of natural carrier oils and aroma chemicals (not "pure essence" — honest branding).

---

## Color Palette

| Token              | Name           | Hex         | Usage                                    |
|--------------------|----------------|-------------|------------------------------------------|
| `--color-bg`       | Forest Dark    | `#071510`   | Page background                          |
| `--color-surface`  | Forest Mid     | `#0D2018`   | Card/surface background                  |
| `--color-elevated` | Forest Light   | `#122A20`   | Elevated/hover states                    |
| `--color-border`   | Forest Border  | `#1A3828`   | Borders and dividers                     |
| `--color-h1`       | White          | `#FFFFFF`   | H1 headings only                         |
| `--color-h2`       | Warm Ivory     | `#F2EBE0`   | H2 and section headings                  |
| `--color-body`     | Sand           | `#E0D9CC`   | Body text and paragraphs                 |
| `--color-nav`      | Warm Gray      | `#C8C2B8`   | Nav links and secondary labels           |
| `--color-muted`    | Sage           | `#9BAAA0`   | Captions, card descriptions, muted text  |
| `--color-gold`     | Gold           | `#F0C842`   | Logo, prices, active links, dividers     |
| `--color-cta`      | Coral          | `#FF8060`   | Primary CTA buttons (Add to Cart, Buy)   |
| `--color-pink`     | Rose           | `#D4889A`   | NEW badge, heart note label              |

## Typography
- **Headings & brand name:** Cormorant Garamond italic (serif, luxury feel)
- **Body, nav, buttons, labels:** Jost (clean sans-serif)
- ~~**Logo/Feature:** Cinzel~~ (removed — no longer used)

## Style Direction
- Luxury minimalism with deep forest green palette
- Generous whitespace
- Photography-forward product showcasing
- Coral accent CTAs for strong conversion contrast
- Gold gradient dividers between sections
- Elegant transitions (300ms)
- High contrast gold on deep green

---

## Final Logo — "The Lane" (option-A-the-lane-v2)

**Chosen logo:** `final logo 2/option-A-the-lane-v2.svg`

**The Story:** "Purani Gali" means "Old Lane." The logo depicts two converging walls in perspective forming a narrow lane, with an arched doorway at the end and golden light spilling through. It represents the journey to discover something rare and precious — an attar shop hidden in the old city.

**Elements:**
- Two perspective walls converging toward a distant arched doorway
- Golden light glow spilling from the archway
- Warm lantern dot inside the arch
- Faint cobblestone ground lines
- "PURANI" (ivory) + "GALI" (gold) below, separated by gold fade lines
- Tagline: "CRAFTED ATTAR" (not "Pure Essence" — honest about blended formulation)

**Integration:**
- Navbar: inline SVG, 120px width, transparent background
- Hero: inline SVG, 260px width, centered, with 5px gap to subtitle
- Footer: text-based "PURANI GALI" + "Crafted Attar"
- No `<img src>` — raw SVG inlined for crisp rendering
- No background `<rect>` — fully transparent, sits on page background

---

## Logo Exploration History

### `logo/` folder — Initial 6 options + story-driven alternatives
| File | Type | Status |
|------|------|--------|
| `option-1-wordmark.svg` | Stacked wordmark | Explored |
| `option-2-monogram.svg` | PG monogram in circle | Explored |
| `option-3-arch-emblem.svg` | Mughal arch + attar drop | Explored |
| `option-3a-arch-bottle.svg` | Arch + bottle outline | Explored |
| `option-3b-arch-monogram.svg` | Arch + PG monogram | Explored |
| `option-4-minimal-bottle.svg` | Bottle icon + name | Explored |
| `option-5-icon-only.svg` | Octagon + drop + PG | Explored |
| `option-6-horizontal-badge.svg` | Horizontal badge | Explored |
| `option-A-the-lane.svg` | Perspective lane | Explored |
| `option-B-the-flame.svg` | Flame + drop | Explored |
| `option-C-the-drop.svg` | Nested 3-layer drop | Explored |
| `option-C1/C2/C3` | Drop refinements | Explored |
| `option-C-key-v3.svg` | Key with "CRAFTED ATTAR" | Explored |

### `final logo/` folder — Key logo iterations
| File | Description |
|------|-------------|
| `option-C-the-key.svg` | Original small key |
| `option-C-key-v2.svg` | Bigger key, bolder strokes |
| `option-C-key-v3.svg` | v2 + "CRAFTED ATTAR" tagline |
| `option-C-key-v4.svg` | 18px gap between key and text |
| `option-C-key-v5.svg` | 8px gap, tightest version |

### `final logo 2/` folder — Final round
| File | Description | Status |
|------|-------------|--------|
| `option-A-the-lane-v2.svg` | Lane logo with "CRAFTED ATTAR" | **FINAL — used on website** |
| `logo-circle-petal.svg` | Circle + petals only (no key) | Alternative |

---

## 3D UI Elements (Spline — CC0 Licensed)

> **Note:** All Spline 3D embeds were removed in the 2026-04-14 rebuild. Kept here for reference if re-adding later.

### 1. Abstract Animation — Interactive Hero Background
- **URL:** https://community.spline.design/file/8b76109f-aea8-42f0-b129-7d354f1ca720
- **Previously used in:** Hero + Experience section backgrounds
- **Status:** Removed

### 2. Radiance — Collection Background
- **URL:** https://community.spline.design/file/2f49f786-6858-40e8-aaa1-29fd35812f0e
- **Previously used in:** Collection section background
- **Status:** Removed

### 3. Perfume Bottle — Interactive Product Spin
- **URL:** https://community.spline.design/file/1d464394-e2fd-4bd7-b6d1-8b536b4576ce
- **Previously used in:** Product Highlight section
- **Status:** Removed

---

## Website Structure

### Pages / Sections
1. **Hero** — Bottle image on left + "Essence of the East" heading + "HANDCRAFTED · NO ALCOHOL" tag + fragrance notes (gold) + description + "Add to Cart" (coral CTA) + "Explore All" (ghost button)
2. **Fragrance Notes Bar** — 3-column layout: Top Note (gold label, Saffron), Heart Note (pink label, Rose Oud), Base Note (muted label, Agarwood)
3. **Collection** — "The Collection" heading + "VIEW ALL" link + 3 product cards:
   - Oud Royale — Agarwood · Amber · Musk — ₹2,499
   - Rose de Nuit — Rose · Sandalwood · Vanilla — ₹1,999 (BESTSELLER badge, gold border)
   - Saffron Noir — Saffron · Patchouli · Oud — ₹3,299 (NEW badge)
4. **Footer** — "Purani Gali · Est. 2025" + scroll-to-top button + Privacy/Shipping/Returns links

### Interactive Elements
- **Scroll animations:** Fade-in on scroll via IntersectionObserver
- **Navbar:** Scroll-triggered compact mode
- **Mobile nav:** Hamburger toggle with slide-in panel

### Features
- Sticky navbar with Lane logo icon + "PURANI GALI" brand name + "CRAFTED ATTAR" tagline + coral "Shop Now" CTA
- Mobile-responsive with hamburger menu (1024px, 768px, 480px breakpoints)
- Scroll-triggered fade-in animations (IntersectionObserver)
- Smooth scroll navigation
- Gold gradient dividers between all sections
- Product cards with BESTSELLER/NEW badges, prices in ₹, coral BUY buttons
- `prefers-reduced-motion` support

---

## Skills Installed

### 1. UI/UX Pro Max
- Path: `.claude/skills/ui-ux-pro-max/SKILL.md`
- Source: https://github.com/nextlevelbuilder/ui-ux-pro-max-skill
- Customized with Attar brand palette, typography, and guidelines
- Provides 50+ design styles, 161 color palettes, 99 UX guidelines

### 2. Canvas Design
- Path: `.claude/skills/canvas-design/SKILL.md`
- Source: https://github.com/anthropics/skills/tree/main/skills/canvas-design
- Used for logo creation — visual art in PNG/PDF/SVG via design philosophy frameworks
- Apache 2.0 licensed, official Anthropic skill

---

## Tech Stack
- HTML5 / CSS3 / Vanilla JavaScript
- Google Fonts (Cormorant Garamond italic, Jost)
- CSS Custom Properties for design tokens
- IntersectionObserver for scroll animations
- Inline SVG logo icon in navbar

## File Structure
```
attar/
├── index.html              — Main website
├── style.css               — All styles with design tokens
├── script.js               — Navbar, animations, form handling
└── assets/
    └── images/
        └── attar-bottle.jpeg  — Product photo

logo/                        — All logo explorations
final logo/                  — Key logo iterations (v1-v5)
final logo 2/                — Final round
├── option-A-the-lane-v2.svg — FINAL LOGO (used on website)
└── logo-circle-petal.svg    — Circle petal alternative

bottle photo/                — Reference bottle image
.claude/skills/              — Installed AI skills
```

## Local Development
```bash
cd attar
python3 -m http.server 3000
# Open http://localhost:3000
```

---

## Deployment
- **Hosted on:** GitHub Pages
- **Live URL:** https://mind-in-code.github.io/purani-gali/
- **GitHub Repo:** https://github.com/Mind-in-code/purani-gali
- **Branch:** `main`, served from root (`/`)
- **Deployed on:** 2026-04-12

---

## Bottle Reference
- Matte black cylindrical rollerball bottle
- Compact, portable design (fits in palm)
- Two straight cylinders: narrower cap on top, wider body below
- Clean seam between cap and body, flat bottom with small notch
- Photo saved in `bottle photo/` folder

## Branding Decisions
- **Tagline:** "CRAFTED ATTAR" (not "Pure Essence" — product uses blended carrier oils + aroma chemicals)
- **Logo choice:** The Lane — represents the brand name literally (Purani Gali = Old Lane) without cultural motifs
- **Legal:** Key logo was analyzed and cleared (low trademark risk in fragrance category) but ultimately not chosen
