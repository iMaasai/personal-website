# loorem.me — Personal Website

The digital representation of Isaac "Loorem" Looremeta — AI, data & analytics leader, Nairobi-born global citizen.

## What this is

A single-file editorial website (`index.html`) — no build step, no dependencies beyond Google Fonts. Open it in a browser or deploy it anywhere static files are served.

## Structure

| File | Purpose | Public? |
|---|---|---|
| `index.html` | The website. Everything: markup, styles, scripts. | ✅ Deployed |
| `README.md` | This file. | ✅ Repo only |
| `isaac_looremeta_360_master_profile.md` | **The source of truth.** Consolidated 360° profile — career, values, journal, vision board, naming rules, content do's/don'ts. All site copy derives from it. | 🔒 Private — never deploy/commit |
| `*.pdf`, `*.jpg`, `*.png` | Source documents: resume, profile PDF, journal & bookshelf photos, podcast screenshots. | 🔒 Private — never deploy/commit |

`.gitignore` and `.vercelignore` enforce the private rows.

## Design system

- **Palette:** deep forest `#0C2018`, warm cream `#F7F3E9`, gold `#C2A04C`, rust `#A4502C` — luxury editorial, per Loorem's design DNA.
- **Type:** Fraunces (display serif) · Space Grotesk (body) · JetBrains Mono (labels) · Caveat (journal pages).
- **Signature elements:** Mount Kenya contour-line hero, site-wide gold-dust physics simulation (pointer-reactive), typewriter name cycle, ultra-running elevation chart, notebook-style journal pages, dawn-ritual arc.
- **Voice:** precise, warm, witty; ruthlessly concise. Third-person references use **Loorem**, never Isaac (full name only for first/formal mention).

## Section map

01 Profile → 02 Three pillars → 03 Selected work → 04 Ventures & public-interest work → 05 What he stands for → 06 The inner work → 07 Beyond the work → 08 Say hello.

## Content rules (the short version)

- Professional framing: **AI, data & analytics** — never AI-only.
- Stoic first; EA is a borrowed toolkit, not an identity.
- Phoenix KE Analytics: member/contributor/mentor — not founder; no "masterclass" references.
- We Run Nairobi (not Urban Swaras). Red Bull/Verstappen (not McLaren).
- It is called **Twitter**.
- Keep private: addresses, family/partner/mentee names, purchase-level details.

Full rules live in the master profile document.

## Deploying

Hosted on Vercel. Redeploy = push to the connected repo, or `vercel deploy` from this folder. `.vercelignore` ensures only the site ships.
