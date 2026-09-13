# XeronOS

Terminal-style personal homepage — single-file `index.html` (vanilla HTML/CSS/JS), zero framework, zero build, zero dependencies.

> Previously `Next.js + React + Tailwind`, rewritten for instant load and free static hosting. Open `index.html` directly in any browser.

![static](https://img.shields.io/badge/stack-vanilla_html-1e1e2e) ![size](https://img.shields.io/badge/size-39KB-cba6f7) ![build](https://img.shields.io/badge/build-none-a6e3a1)

## Preview

All-English light editorial one-pager. Three distinct interaction languages: **Selected Work** rows spawn a floating preview card (real GitHub OG image) that trails the cursor with damped physics and velocity tilt, the row name turning blue italic with an underline draw; **Writing** rows keep the ink-fill wipe; **Contact** is a wall of giant outline serif words (BLOG / GITHUB / X / TELEGRAM / EMAIL) that fill solid on hover while a klein-blue marquee strip scrolls the handle through the letters — email click copies to clipboard and the cursor label flips to "COPIED" (touch devices get a clean outline word + handle fallback instead). Plus: loader counter (000→100) → curtain lift → per-letter hero rise with cursor-proximity kinetic letters → section titles text-scramble on reveal → scroll-velocity skew on lists → film grain, scroll progress bar. Honors `prefers-reduced-motion`. Radically minimal copy — only the name, the thesis, the work, the writing, the stack, the contact. Content drawn from GitHub — ArchdevilForge org repos first, then personal (28 + 9) — the blog (27 essays) and X.

> Earlier terminal/fastfetch version lives in git history (`git log --oneline`).

## Edit

All content is in one file:

- **System info / links / colors** → `:root` CSS variables (Catppuccin Mocha) and HTML in `index.html`
- **No build step** — edit and refresh

## Deploy

Any static host works. No `npm install`, no `next build`:

- **Vercel** — Framework Preset → `Other`, Build Command empty, Output `.` (already set in `vercel.json`)
- **Cloudflare Pages / Netlify / GitHub Pages** — upload `index.html`

## Stack

`HTML + CSS + 30 lines JS` — typewriter + `Intl.DateTimeFormat` clock. No React, no bundler.
