# AI Frontend Design Skills

Free and open source Agent Skills for building better frontend websites, landing pages, business websites, ecommerce layouts, and WordPress themes with AI coding agents.

This skill pack was distilled from `372 website/theme packages analyzed`. It does not include original theme ZIPs, copied code, images, fonts, demo content, or bundled plugins. It contains only reusable guidance, workflows, and references that help an AI agent design and build original work.

## What Is Inside

- 3 ready-to-use skills.
- 4 reference guides.
- Codex UI metadata in `agents/openai.yaml`.
- MIT license.
- Clean Markdown files prepared for GitHub publishing.

## Included Skills

### `frontend-design-master`

Use this skill to build polished frontend websites and WordPress-style themes for any niche: clinics, agencies, restaurants, real estate, hotels, education, portfolios, ecommerce, local services, nonprofits, SaaS pages, and more.

It helps with:

- Page structure and section planning.
- Hero sections, headers, service grids, trust bands, contact sections, and footers.
- Responsive design systems.
- Business website layouts.
- Landing pages and conversion flows.
- Ecommerce and product-grid layout ideas.
- WordPress theme planning without copying existing themes.

### `wp-theme-pattern-miner`

Use this skill to inspect WordPress theme folders or ZIP collections and extract reusable frontend ideas safely.

It helps with:

- Counting and classifying theme packages.
- Finding common WordPress theme structures.
- Learning from headers, sliders, front-page sections, templates, Customizer options, and ecommerce files.
- Turning old theme patterns into modern original frontend guidance.

### `frontend-visual-polish`

Use this skill to review and refine a frontend before delivery.

It helps with:

- Mobile and desktop layout checks.
- Typography, spacing, and color polish.
- Text overflow and visual hierarchy.
- Screenshot-based QA.
- Interaction states, forms, buttons, and responsive menus.
- Final production-readiness review.

## Main Features

- Helps AI agents build frontend websites from clear design rules.
- Helps create WordPress themes for whatever niche or business type you want.
- Supports landing pages, full business websites, ecommerce sections, portfolios, blogs, and local service sites.
- Converts large theme collections into reusable design patterns.
- Keeps public outputs clean by avoiding copied original assets.
- Works as a reusable skill pack for Codex and Claude/Agent Skills compatible tools.
- Free and open source under the MIT license.

## How To Use With Codex

Copy one skill folder into your Codex skills folder:

```powershell
Copy-Item -Recurse .\skills\frontend-design-master "$env:USERPROFILE\.codex\skills\frontend-design-master"
```

Then ask Codex to use it:

```text
Use $frontend-design-master to build a modern WordPress theme concept for a real estate website.
```

You can also install the other skills:

```powershell
Copy-Item -Recurse .\skills\wp-theme-pattern-miner "$env:USERPROFILE\.codex\skills\wp-theme-pattern-miner"
Copy-Item -Recurse .\skills\frontend-visual-polish "$env:USERPROFILE\.codex\skills\frontend-visual-polish"
```

## How To Use With Claude Or Other Agent Skills Tools

Each skill is a standalone folder with:

- `SKILL.md`
- optional `references/`
- optional `agents/openai.yaml`

For tools that import ZIP files, zip one skill folder at a time. Example:

```text
skills/frontend-design-master
```

## Example Prompts

```text
Use $frontend-design-master to design a clean WordPress theme for a dental clinic.
```

```text
Use $wp-theme-pattern-miner to analyze this WordPress theme folder and extract reusable layout ideas.
```

```text
Use $frontend-visual-polish to review this landing page and make it look production-ready on mobile and desktop.
```

 # About 
AI Frontend Design Skills is a free and open source skill pack for AI coding agents. It helps agents build polished frontend websites, WordPress themes, landing pages, ecommerce layouts, business websites, and responsive UI systems for any niche.

The pack was distilled from 372 website/theme packages analyzed. It includes 3 skills, 4 reference guides, Codex metadata, and an MIT license. No original theme ZIPs, copied code, images, fonts, demo content, or bundled plugins are included.

Use it with Codex, Claude, or any Agent Skills compatible workflow to plan, build, analyze, and polish original frontend work.
