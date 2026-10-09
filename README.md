# TGSUM product site

Russian product landing and reusable React component kit, with a fully synthetic, interactive product demonstration.

## Run locally

```sh
npm ci
npm run dev -- --host 0.0.0.0 --port 4173 --strictPort
```

## Production

```sh
npm run build:pages
npm test
```

The static site is emitted to `dist/client`; `npm run build:pages` also copies it to `docs/`, the GitHub Pages publishing source (main branch, /docs folder). Vite's base path is `/tgsum-site/` for GitHub Pages. All assets, including Cyrillic variable fonts, are self-hosted. No analytics, external runtime API requests, login, or account connections are included.

## Components

See [COMPONENTS.md](COMPONENTS.md). Components are in `src/components.jsx`; design tokens and responsive styles are in `src/styles.css`. The live component gallery is at `#components`.

## Public product evidence

Verified 2026-10-09 against public development commit `f34906a55a219999f395def0ec9b51a02d68e1cb`:

- [Product README](https://github.com/Roflochinsky/tgsum/blob/f34906a55a219999f395def0ec9b51a02d68e1cb/README.md)
- [Cloud workflow](https://github.com/Roflochinsky/tgsum/blob/f34906a55a219999f395def0ec9b51a02d68e1cb/docs/development/cloud-workspace.md)
- [Privacy controls](https://github.com/Roflochinsky/tgsum/blob/f34906a55a219999f395def0ec9b51a02d68e1cb/docs/development/privacy-controls.md)
- [Context packages](https://github.com/Roflochinsky/tgsum/blob/f34906a55a219999f395def0ec9b51a02d68e1cb/docs/development/local-package-mvp.md)
- [Evidence validation update](https://github.com/Roflochinsky/tgsum/commit/f34906a55a219999f395def0ec9b51a02d68e1cb)

New desktop and cloud-workspace features are explicitly described as development/experimental capabilities. This site does not imply that those features are in the older public CLI release. AI results require review; local preparation and optional cloud transfer are clearly distinguished.

## Demo data and privacy

All example messages, task owners, dates, counts, and summaries are invented. Nothing is uploaded when interacting with the demo. The Markdown download contains only those same invented examples. No private repository data, credentials, customer information, or real conversations are included.

## Design and credits

Visual direction supplied by the user: [Atharvsinh-codez/Project-1](https://github.com/Atharvsinh-codez/Project-1), live reference [Project-1](https://project-one.obsidianui.dev/). This is an original implementation following its cream palette, bold typography, floating black navigation, tactile hero art and generous composition. No source code or assets from that repository are redistributed.

- Hero image: original AI-generated illustration created for this site.
- UI icons: Phosphor Icons, MIT license.
- Typeface: Manrope, SIL Open Font License, served locally via Fontsource.

This is a product presentation and frontend demo, not the actual TGSUM application or a backend integration.
