# loorem.fyi — Personal Website

The digital representation of Isaac "Loorem" Looremeta — AI, data & analytics leader, Nairobi-born global citizen.

**Status: 🟢 live at [loorem.fyi](https://loorem.fyi) since July 2, 2026.** Indexed with Google Search Console; Vercel Web Analytics + Speed Insights tracking.

## What this is

A single-file editorial website (`index.html`) — no build step, no dependencies beyond Google Fonts and Vercel's first-party analytics snippets. Open it in a browser or deploy it anywhere static files are served.

## Structure

| File | Purpose | Public? |
|---|---|---|
| `index.html` | The website. Everything: markup, styles, scripts. | ✅ Deployed |
| `README.md` | This file. | ✅ Repo only |
| `isaac_looremeta_360_master_profile.md` | **The living source of truth.** Consolidated 360° profile — career, values, journal, vision board, naming rules, content do's/don'ts. Current resumes and role documents supersede older professional details and should be propagated here. | 🔒 Private — never deploy/commit |
| `*.pdf`, `*.jpg`, `*.png` | Source documents: resume, profile PDF, journal & bookshelf photos, podcast screenshots. | 🔒 Private — never deploy/commit |
| `og-image.png` | Generated social-share card (the sole image exception, whitelisted by name). | ✅ Deployed |

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

Hosted on Vercel, imported from the private GitHub repo `iMaasai/personal-website` — every push to `main` auto-deploys. `.vercelignore` ensures only the site ships.

**Live URL:** https://loorem.fyi — the only public URL. The `*.vercel.app` address is behind Vercel deployment protection (SSO) by design.

## Google Search Console (✅ completed July 2026 — kept as a runbook)

1. Confirm https://loorem.fyi loads with valid SSL (Vercel provisions the cert automatically once DNS propagates).
2. Go to [search.google.com/search-console](https://search.google.com/search-console) → **Add property** → choose **Domain** type → enter `loorem.fyi`. Domain properties cover www/non-www and http/https in one go.
3. Google shows a TXT record (`google-site-verification=…`). Add it in Vercel: **Dashboard → Domains → loorem.fyi → DNS Records → Add** — type `TXT`, name blank (root), paste the value. Back in Search Console, click **Verify** (may take a few minutes for the record to propagate).
4. Once verified: **URL Inspection** → enter `https://loorem.fyi/` → **Request indexing**. That's the whole job for a single-page site — no sitemap needed for one URL.
5. Optional, later: check **Performance** after a few weeks to see what queries surface the site; confirm the canonical is recognized under **Pages**.

## Next steps

Launch scope is complete (domain, SSL, Search Console, analytics, 2FA — all ✅ July 2026). What remains is off-site or parked:

1. **Align external profiles with the current professional positioning** — LinkedIn, Gleac, about.me, Torre, ResearchGate, and X/IG bios. Propagate: exact Numida title (**Applied AI & Analytics Lead**), senior-IC and measured-outcome framing, VelocityStack's assessment-led Build / Train / Operate model, and Phoenix role (member/contributor/mentor).
2. **Content ideas parked for later** — Strava embed/live stats, photo touches from the bookshelf/journal scans, a writing/notes section if he starts publishing.
