# stark-hq-web — Coming Soon Pages

## Overview
Two standalone coming-soon landing pages for Cloudflare Pages.
Pure HTML/CSS/JS only — NO frameworks, NO build tools, NO npm.
Each site is a single `index.html` file in its own subdirectory.

## Repo Structure
```
stark-hq-web/
├── starkforge/
│   └── index.html
├── starkrobotics/
│   └── index.html
└── CLAUDE.md
```

## Deployment
- Cloudflare Pages — static hosting
- Each subdirectory deploys independently as its own site
- No server-side code, no build step

---

## Site 1: StarkForge (`starkforge/index.html`)

**Domain:** starkforge.ai  
**Tagline:** The Intelligence Layer for the Agentic Fleet  
**Brand accent:** Electric cyan `#00d4ff`  
**Theme:** Dark, technical, futuristic  

### Design Spec
- Full-viewport dark background (`#050a0f` or similar near-black)
- Animated canvas background: node/edge network (particles connected by lines, slowly drifting)
- Logo/wordmark: `STARKFORGE` in bold geometric sans-serif, electric cyan
- Tagline below: `The Intelligence Layer for the Agentic Fleet` — white, lighter weight
- "Coming Soon" badge — subtle, monospace or small caps
- Contact line: `info@starkforge.ai` — dimmed, bottom of page or below tagline
- NO countdown timer
- NO email capture form
- `prefers-reduced-motion`: disable canvas animation, keep static layout

### Color Palette
- Background: `#050a0f`
- Primary accent: `#00d4ff` (electric cyan)
- Secondary: `#0088aa` (darker cyan for depth)
- Text primary: `#ffffff`
- Text muted: `#6b8599`
- Node color: `#00d4ff` at low opacity
- Edge color: `rgba(0, 212, 255, 0.15)`

---

## Site 2: StarkRobotics (`starkrobotics/index.html`)

**Domain:** starkrobotics.ai  
**Tagline:** Building the Machines of Tomorrow  
**Brand accent:** Steel orange `#ff6b2b`  
**Theme:** Dark, industrial, heavy  

### Design Spec
- Full-viewport dark background (`#0a0805` or similar warm near-black)
- Background texture: CSS circuit grid (fine lines forming a grid pattern, subtle)
- Logo/wordmark: `STARKROBOTICS` in bold geometric sans-serif, steel orange
- Tagline below: `Building the Machines of Tomorrow` — white, lighter weight
- "Coming Soon" badge — subtle, monospace or small caps
- Contact line: `info@starkrobotics.ai` — dimmed, bottom of page or below tagline
- NO countdown timer
- NO email capture form
- Optional: subtle scanline or industrial texture overlay
- `prefers-reduced-motion`: disable any animation, keep static layout

### Color Palette
- Background: `#0a0805`
- Primary accent: `#ff6b2b` (steel orange)
- Secondary: `#cc4400` (darker orange for depth)
- Text primary: `#ffffff`
- Text muted: `#8a7060`
- Grid lines: `rgba(255, 107, 43, 0.08)`

---

## Quality Bar
- Works in Chrome, Firefox, Safari (modern versions)
- Responsive — looks great on mobile and desktop
- No external dependencies (no Google Fonts CDN, no icon libraries)
  - Embed any fonts as base64 or use system font stack
  - Use CSS-only icons/shapes where needed
- Passes basic a11y: semantic HTML, alt text on any images, contrast ratios
- Each file should be self-contained (no external CSS/JS imports)
- Minification NOT required — readable code preferred

## Code Style
- Clean, well-commented HTML/CSS/JS
- CSS custom properties (variables) for colors
- Vanilla JS only for canvas animations
- No jQuery, no React, no Tailwind
