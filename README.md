# AI Radiology Assistant — Landing Page

[![Deploy to GitHub Pages](https://github.com/kazdatahelp/radiology-ai-landing/actions/workflows/deploy.yml/badge.svg)](https://github.com/kazdatahelp/radiology-ai-landing/actions/workflows/deploy.yml)

🌐 **Live Site:** [https://kazdatahelp.github.io/radiology-ai-landing/](https://kazdatahelp.github.io/radiology-ai-landing/)

--- 

## Overview

Marketing landing page for **AI Radiology Assistant** — an AI-powered CT analysis system for Kazakhstan healthcare.

### Features

- 🌍 **Bilingual** — Russian and English with instant toggle
- 📱 **Responsive** — Works on all devices
- ⚡ **Fast** — Single HTML file, no build step required
- 🎨 **Modern Design** — Dark medical-tech aesthetic with animations

---

## Quick Start

### Local Preview

Simply open `index.html` in your browser:

```bash
# macOS
open index.html

# Linux
xdg-open index.html

# Windows
start index.html
```

### Deploy to GitHub Pages

1. Fork or clone this repository
2. Go to **Settings** → **Pages**
3. Source: **GitHub Actions**
4. The site will auto-deploy on every push to `main`

---

## Project Structure

```
radiology-ai-landing/
├── index.html              # Main landing page (self-contained)
├── README.md               # This file
├── assets/
│   └── images/             # Add screenshots, logos here
│       └── .gitkeep
└── .github/
    └── workflows/
        └── deploy.yml      # GitHub Pages deployment
```

---

## Customization

### Update Content

Edit `index.html` directly. The page uses CSS variables for easy theming:

```css
:root {
  --slate-900: #0f172a;    /* Background */
  --cyan-500: #06b6d4;     /* Primary accent */
  --cyan-400: #22d3ee;     /* Hover states */
  /* ... */
}
```

### Add Images

1. Place images in `assets/images/`
2. Reference in HTML:
   ```html
   <img src="assets/images/screenshot.png" alt="...">
   ```

### Custom Domain

1. Add your domain to `CNAME` file:
   ```
   radiology-ai.kz
   ```
2. Configure DNS with your domain registrar

---

## Sections

| Section | Description |
|---------|-------------|
| Hero | Value proposition + animated CT visualization |
| Problem | Pain points + time comparison (20 min → 3 min) |
| Features | 6 key capabilities |
| Workflow | 3-step process |
| Metrics | PoC target KPIs |
| Integrations | PACS Akgun & Damumed |
| Pricing | 3 pricing tiers |
| CTA | Contact form |

---

## Related Repositories

- **Main Project:** [ai-radiology-assistant-poc](https://github.com/kazdatahelp/ai-radiology-assistant-poc) (private)

---

## Tech Stack

- Pure HTML5 + CSS3 + Vanilla JavaScript
- No dependencies, no build step
- Google Fonts (DM Sans)
- SVG icons and animations

---

## License

© 2025 AI Radiology Assistant. All rights reserved.

---

## Contact

📧 info@radiology-ai.kz
