# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this is

A zero-dependency single-file personal website (`index.html`) — markup, styles, and scripts all in one file. No build step. Open in a browser or deploy anywhere static files are served.

Live at **https://loorem.fyi** (the only public URL — the `*.vercel.app` address is SSO-protected by design).

## Developing

Open `index.html` directly in a browser. There is no build, no package manager, no dev server required.

To deploy:

```
vercel deploy
```

Or push to the connected Vercel repo — it redeploys automatically. `.vercelignore` ships only `index.html` and `og-image.png`.

## Architecture

Everything lives in `index.html`. Section order:

`#top` (hero) → `#about` → `#pillars` → `#work` → `#ventures` → `#values` → `#practice` → `#beyond` → `#contact`

Interactive features all run as vanilla JS in a `<script>` at the bottom: gold-dust physics canvas (pointer-reactive), typewriter name cycle (`#aka`), SVG contour-line hero, ultra-running elevation chart, mobile hamburger menu (full-screen overlay below 920px, with focus trap and scroll lock). Vercel Web Analytics + Speed Insights load via first-party `/_vercel/*/script.js` snippets — no npm packages.

## Content source of truth

`isaac_looremeta_360_master_profile.md` is the master document — all site copy, naming rules, values framing, and content do's/don'ts derive from it. **Read it before editing any site copy.** For current professional titles, dates, scope, and achievements, the latest resume and role documentation supersede older profile language; update the master profile alongside the site. The master profile is `.gitignore`d and `.vercelignore`d; never commit or deploy it.

## Content rules (short version)

- Professional framing: **AI, data & analytics** — never AI-only.
- Third-person: **Loorem** throughout; full name "Isaac Looremeta" only for first or formal mention.
- Stoic first; EA is a borrowed toolkit, not an identity.
- Phoenix KE Analytics: member/contributor/mentor — not founder; no "masterclass" references.
- Numida role: use the exact title **Applied AI & Analytics Lead** (from August 2026). It is a **senior IC**, not a line-management or team-head role; describe focused, end-to-end ownership through measured impact.
- We Run Nairobi (not Urban Swaras). Red Bull/Verstappen (not McLaren). It is called **Twitter**.
- Never include: addresses, family/partner/mentee names, purchase-level details.

## Design system

- **Palette:** deep forest `#0C2018`, warm cream `#F7F3E9`, gold `#C2A04C`, rust `#A4502C`
- **Fonts:** Fraunces (display serif) · Space Grotesk (body) · JetBrains Mono (labels) · Caveat (journal pages) — loaded via Google Fonts
- **Voice:** precise, warm, witty; ruthlessly concise.

## Privacy boundary

`.gitignore` and `.vercelignore` both enforce that `*.pdf`, `*.jpg`, `*.jpeg`, `*.png`, and all `isaac_looremeta_*.md` files are never committed or deployed. Do not change these rules. Sole exception, approved July 2026: `og-image.png` (the generated social-share card) is whitelisted by exact name in both files — do not remove that exception, and do not add further ones without explicit approval.
