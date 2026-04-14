# PROJECT_CONTEXT.md — Purani Gali

## Overview
Luxury single-page website for **Purani Gali**, a crafted attar (oil-based perfume) brand. Dark, premium aesthetic with interactive 3D elements. The brand uses blended carrier oils + aroma chemicals — branded honestly as "Crafted Attar."

## Tech Stack
- **Plain HTML5 / CSS3 / Vanilla JavaScript** — no frameworks, no bundlers, no build step
- **Google Fonts:** Cormorant Garamond (italic), Jost
- **Spline 3D** embeds (iframe) — interactive + ambient backgrounds
- **Canvas API** — gold particle system (oud smoke)
- **CSS Custom Properties** — design tokens for colors, fonts, easing
- **IntersectionObserver** — scroll-triggered animations
- **Local dev:** `cd attar && python3 -m http.server 3000`

## What's Built
- Streamlined single-page site with 4 sections: Hero, Fragrance Notes Bar, Collection (product cards), Footer
- Hero: bottle image + "Essence of the East" heading + "Add to Cart" / "Explore All" CTAs
- Fragrance Notes Bar: Top/Heart/Base notes in 3 columns with colored labels (gold/pink/muted)
- Collection: 3 product cards (Oud Royale ₹2,499, Rose de Nuit ₹1,999, Saffron Noir ₹3,299) with BESTSELLER/NEW badges, BUY buttons
- Navbar: Lane logo icon + "PURANI GALI" brand name + "CRAFTED ATTAR" tagline + nav links + coral "Shop Now" CTA
- Footer: "Purani Gali · Est. 2025", scroll-to-top button, Privacy/Shipping/Returns links
- Gold gradient dividers between all sections
- Responsive design (1024px, 768px, 480px breakpoints)
- Mobile hamburger nav with slide-in panel
- `prefers-reduced-motion` support
- Sticky navbar with scroll effect
- IntersectionObserver fade-in animations

## Deployment
- **Live URL:** https://mind-in-code.github.io/purani-gali/
- **GitHub Repo:** https://github.com/Mind-in-code/purani-gali
- **Hosting:** GitHub Pages (main branch, root `/`)

## What's Pending
- No backend — contact form doesn't actually submit
- No e-commerce / product pages
- No SEO meta tags, favicon, or analytics
- No cookie consent / privacy policy
- Real product photography (currently using Spline 3D bottle)

## Key Decisions
- **"Crafted Attar"** over "Pure Essence" — honest branding
- **The Lane logo** — represents "Purani Gali" (Old Lane) literally
- **Inline SVG** logos — no `<img>` tags, transparent backgrounds
- **Zero dependencies** — vanilla JS only, no libraries
- **Spline 3D via iframe** — CC0 licensed community assets for premium feel

## Changelog
- **2026-04-12:** PROJECT_CONTEXT.md created. Website is fully built — all 8 sections, 4 Spline embeds, particle system, responsive layout, Lane logo integrated.
- **2026-04-12:** Deployed to GitHub Pages. Live at https://mind-in-code.github.io/purani-gali/. Repo: Mind-in-code/purani-gali.
- **2026-04-14:** Complete site rebuild to match new design reference. Removed Spline 3D embeds, particle canvas, About/Experience/Product Highlight/Testimonials/Contact sections. New structure: Hero (bottle + heading + dual CTAs), Fragrance Notes Bar (3-column), Collection (3 product cards with prices/badges/buy buttons), minimal footer. New design system: forest green palette (#071510/#0D2018), gold #F0C842, coral CTA #FF8060, pink badge #D4889A. Typography: Cormorant Garamond italic headings, Jost body. Removed Cinzel font.
