# Digital Product Passport — Mock Prototype

A static, mobile-first Digital Product Passport (DPP) for **Knauf Insulation Mineral Wool 035 Light**, built as a single-page web application.

## Quick Start

Open `index.html` in any modern browser — no build step, no server required.

```bash
# Or serve locally for a more realistic experience:
npx serve .
# Then open http://localhost:3000
```

## What This Is

A mock DPP prototype simulating the experience of scanning a QR code on a physical construction product and landing on `dpp.earth/4003950138263`. All data is based on real EPD data (S-P-03779) for Knauf Insulation Mineral Wool 035 Light.

## Sections

1. **Product Identity** — manufacturer, GTIN, CE marking, EPD reference
2. **GWP Hero** — animated Global Warming Potential with A1/A2/A3 breakdown
3. **19 CPR Environmental Indicators** — collapsible by regulatory phase (2026/2030/2032)
4. **Recycled Content & Material Composition** — 58% recycled content ring + doughnut chart
5. **Technical Performance** — thermal conductivity, density, fire class
6. **Lifecycle Scope** — module pipeline (A1–D) with coverage indicators
7. **Circularity & End-of-Life** — locked preview (role-based access demo)
8. **BIM Integration** — locked preview (role-based access demo)
9. **Footer** — passport metadata, self-referential QR code, Emidat branding

## Features

- Mobile-first responsive design
- Dark/light mode toggle (respects system preference)
- Scroll-triggered animations (counter, ring, fade-ins)
- Print stylesheet (Download as PDF via browser print)
- QR code generation
- EN/DE language toggle (UI placeholder)
- Zero build step — single HTML file with CDN dependencies

## Dependencies (loaded via CDN)

- [Inter font](https://fonts.google.com/specimen/Inter) — Google Fonts
- [Chart.js 4](https://www.chartjs.org/) — doughnut chart
- [qrcode-generator](https://github.com/niclas21/qrcode-generator) — footer QR code

## Design System

| Token | Value |
|---|---|
| Primary green | `#C8E84E` |
| Dark | `#1A1A2E` |
| Surface | `#F5F5F7` |
| Font | Inter, system sans-serif |
| Border radius | 12px (cards), 8px (small), 6px (xs) |

## Deployment

Drop `index.html` into any static host:

- **Netlify**: drag and drop the folder
- **Vercel**: `vercel --prod`
- **GitHub Pages**: push to a `gh-pages` branch

## Context

Built for Emidat lighthouse customer discovery meetings. Demonstrates how verified EPD data transforms into a Digital Product Passport under EU CPR 2024/3110 and ESPR 2024/1781.
