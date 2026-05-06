# CPM GrapesJS — Christiano Property Management Live Editor

A production-configured [GrapesJS](https://grapesjs.com/) visual editor preloaded with the CPM homepage and pricing section. Built for non-technical clients to edit live content with zero code.

---

## Features

- **Live visual editing** — drag, drop, and edit text/sections directly on the page
- **Two pages preloaded** — Homepage and Pricing Section, switchable via top bar
- **Auto-save** — saves to `localStorage` every 60 seconds
- **Manual save** — `Ctrl/Cmd + S` or the Save button
- **Export HTML** — download clean, self-contained HTML per page
- **Undo/Redo** — `Ctrl/Cmd + Z` / `Ctrl/Cmd + Y`
- **Device preview** — Desktop, Tablet, Mobile
- **Full plugin suite** — 13 plugins including forms, tabs, countdown, custom code, touch, tooltips, image editor
- **CPM gold theme** — branded dark UI with `#c9a96e` gold accents

## Plugins Included

| Plugin | Purpose |
|--------|---------|
| `grapesjs-preset-webpage` | Full webpage editing preset |
| `grapesjs-blocks-basic` | Core drag-and-drop blocks |
| `grapesjs-plugin-forms` | Form components |
| `grapesjs-component-countdown` | Countdown timers |
| `grapesjs-plugin-export` | HTML export |
| `grapesjs-tabs` | Tab components |
| `grapesjs-custom-code` | Embed raw HTML/JS |
| `grapesjs-touch` | Mobile touch support |
| `grapesjs-parser-postcss` | PostCSS parsing |
| `grapesjs-tooltip` | Tooltip components |
| `grapesjs-tui-image-editor` | In-editor image editing |
| `grapesjs-typed` | Typed.js text animation |
| `grapesjs-style-bg` | Background style manager |

## Usage

### Quick Start (No build needed)

```bash
git clone https://github.com/CerisonAutomation/cpmgrapejs.git
cd cpmgrapejs
npx serve .
```

Or simply open `index.html` directly in any browser.

### Deploy on Vercel (Recommended)

1. Push this repo to GitHub (already done)
2. Go to [vercel.com](https://vercel.com) → New Project → Import `cpmgrapejs`
3. Framework: **Other** (static)
4. Deploy — live URL in under 60 seconds

## Pages

| Page | Description |
|------|-------------|
| **Homepage** | Full CPM homepage — hero, process, portfolio, contact |
| **Pricing Section** | Management Plans — Essentials & Premium tiers |

## Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| `Ctrl/Cmd + S` | Save current page |
| `Ctrl/Cmd + Z` | Undo |
| `Ctrl/Cmd + Y` | Redo |

## Architecture

- Zero build step — single `index.html`, CDN-loaded GrapesJS
- `localStorage` persistence per page key (`cpm_gjs_homepage`, `cpm_gjs_pricing`)
- Export produces clean standalone HTML files

## Based On

- [GrapesJS](https://github.com/GrapesJS/grapesjs) — Open-source web builder framework (forked: [CerisonAutomation/grapesjs](https://github.com/CerisonAutomation/grapesjs))

## License

MIT
