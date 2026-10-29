# Grupo APEX Americas — Company Profile 2026

Bilingual (ES / EN) web presentation of Grupo APEX Americas (MAG · APAMO · Avanza).

Static site — no build step.

## Structure
```
index.html            The deck (9 slides, 1280×720, auto-scaled)
assets/apex-logo.png    Grupo APEX logo
assets/apamo-logo.png   ApaMo logo
assets/avanza-logo.png  Avanza logo
assets/brands/          Carmaker logos
assets/favicon.png      Browser tab icon
vercel.json           Hosting headers (noindex)
```

## Deploy on Vercel
1. Push this folder to a new GitHub repository.
2. In Vercel: **Add New → Project → Import** the repo.
3. Framework preset: **Other**. Leave build command and output directory empty.
4. Deploy.

## Use
- Password: set in `index.html` → `var PASSWORD = 'APEX2026';`
  (client-side gate only — it keeps casual visitors out, it is not real security)
- Navigate with ← → arrow keys, the on-screen buttons, or swipe on mobile.
- Toggle ES / EN with the switch at top right.
- Link directly to a slide with `#n` (e.g. `/#6`).
- Export to PDF: browser **Print → Save as PDF** (one slide per page).

## Carmaker logos (slide 4)
All carmaker logos are wired in. To change or add one:
1. Put the files in `assets/brands/` (PNG or SVG, transparent background), e.g. `toyota.png`.
2. In `index.html`, find `var BRAND_LOGOS` and uncomment / add the matching lines.
Keys: toyota, ford, chrysler, jeep, ram, dodge, chevrolet, international, gm.
