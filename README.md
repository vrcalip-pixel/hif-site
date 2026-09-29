# Human Intelligence Festival — landing page

Immersive single-page site for the LARC Human Intelligence Festival (Nov 6, 2026, The Magic Box, DTLA).
Live at https://humanintelligencefestival.la (GitHub Pages).

## Structure
- `index.html` — the whole site: pinned 3D scroll scene, orb navigation, overlay panels (`#expect`, `#students`, `#faculty`, `#employers`, `#sponsor`, `#register`), Ambiance toggle.
- `assets/hero.webp` — banner used for the reduced-motion / no-JS fallback (and social previews).
- `CNAME` — custom domain for GitHub Pages. Do not delete.

## Dependencies (CDN only, no build step)
- GSAP 3.12.5 + ScrollTrigger (cdnjs)
- Google Fonts: Outfit

## Editing content
All copy lives in the overlay panels near the bottom of `index.html`. Sponsorship tiers are in `#ov-sponsor`.
Registration form is a prototype: point `#regform` at a real endpoint (Formspree, Google Form, Eventbrite embed) before launch.
Ambiance music: drop a licensed MP3 in `assets/` and set `src` on `<audio id="ambTrack">`; the generative synth is used only when no `src` is set.

## Deploy
Push to `main`. GitHub Pages serves the root of `main`.
