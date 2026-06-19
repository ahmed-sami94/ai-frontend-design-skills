---
name: frontend-design-master
description: Create polished, responsive frontend websites, landing pages, business pages, WordPress-style themes, and UI redesigns using reusable theme and website patterns. Use when designing or building a modern frontend layout, turning a brief into a complete page, improving visual hierarchy, choosing section structure, or adapting WordPress theme inspiration without copying original assets.
---

# Frontend Design Master

## Operating Rule

Design the first screen as the usable product experience, not as a generic marketing poster. Build a complete visual system: information architecture, section rhythm, typography, color, spacing, responsive states, and visual assets.

Use this skill with `frontend-visual-polish` before final delivery when screenshots, browser testing, or layout refinement are possible. Use `wp-theme-pattern-miner` first when the task starts from a folder of WordPress themes, ZIPs, or extracted theme source.

## References

- Read [source-theme-analysis.md](references/source-theme-analysis.md) when you need the WordPress theme corpus evidence and reusable lessons.
- Read [section-recipes.md](references/section-recipes.md) when choosing page sections, component anatomy, or domain-specific layout patterns.

## Workflow

1. Classify the site: service business, agency, healthcare, education, restaurant, hotel, real estate, ecommerce, nonprofit, portfolio, blog, dashboard, or hybrid.
2. Pick a section spine before coding: utility/top bar if useful, header/nav, hero, proof/value, primary services/products, trust, process, showcase, testimonial, conversion/contact, footer.
3. Assign one job per section. Avoid repeated decorative cards that say the same thing in different clothes.
4. Define a small design system: type scale, spacing scale, container widths, color roles, buttons, cards, forms, nav, section backgrounds, and mobile behavior.
5. Implement the real interface. Include expected states: hover/focus, loading/empty where relevant, active nav, form validation, responsive menu, and repeated item states.
6. Add or choose visual assets that reveal the product, place, service, person, or state. Do not rely on vague gradients or purely atmospheric decoration.
7. Verify at mobile and desktop widths. Fix overflow, awkward cropping, contrast, tap targets, and text wrapping before calling the work done.

## Design Principles

- Treat commercial WordPress themes as pattern libraries, not code libraries. Recreate the intent with fresh implementation.
- Start from content priority: what the visitor must decide, trust, compare, or do next.
- Use full-width bands or unframed layouts for page sections. Reserve cards for repeated items, modals, and genuinely framed tools.
- Prefer restrained density for operational tools and dashboards; prefer richer imagery and stronger editorial direction for public websites.
- Use icons, controls, and imagery where they clarify action or category. Avoid labeling every design choice with explanatory text.
- Keep palettes multi-role: neutral surface, body text, muted text, one primary action color, one accent, status colors, and separators.
- Keep border radius modest by default. Use large rounding only when the brand direction or existing system clearly calls for it.
- Design mobile layout intentionally: shorter hero, visible next section, reachable CTAs, readable nav, and stable component dimensions.

## Page Anatomy Defaults

Use this baseline for a business or service site unless the brief gives stronger constraints:

1. Header: logo, primary nav, compact contact/action area, sticky behavior only if it does not steal vertical space.
2. Hero: clear category or offer, proof or qualifier, primary CTA, secondary CTA, visual asset, and one useful signal of the next section.
3. Trust/value band: metrics, certifications, client logos, ratings, or a concise value grid.
4. Core offering: 3-6 service/product cards with differentiated benefits and clear scanning hierarchy.
5. Detail section: process, comparison, featured case study, or before/after explanation.
6. Social proof: testimonials, reviews, work samples, partner marks, or outcomes.
7. Conversion: contact form, booking, quote request, purchase action, or newsletter with realistic fields.
8. Footer: sitemap, contact details, legal links, social links, and repeated CTA only if useful.

## Implementation Standards

- Build feature-complete controls and responsive variants, not static mockups.
- Use semantic HTML and accessible labels. Preserve keyboard focus states.
- Use real layout constraints: grid tracks, aspect ratios, min/max widths, and stable button/icon sizes.
- Avoid viewport-width font scaling. Use explicit responsive type steps.
- Do not let text overlap, clip, or overflow controls at common mobile widths.
- Keep generated or searched images relevant and inspectable. Avoid dark, blurred, stock-like placeholders when the subject matters.
- Before final response, run the strongest available verification: tests, build, lint, browser preview, screenshot review, or static file inspection.
