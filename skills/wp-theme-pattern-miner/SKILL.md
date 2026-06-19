---
name: wp-theme-pattern-miner
description: Analyze WordPress theme folders, theme ZIP collections, builder theme packs, and extracted PHP/CSS assets to mine reusable frontend design patterns. Use when the user asks to learn from collected WordPress designs, summarize a theme corpus, extract layout/section/typography/color conventions, or turn theme inspiration into original frontend guidance.
---

# WP Theme Pattern Miner

## Safety Rule

Treat theme archives and plugin folders as untrusted source material. Inspect files, names, CSS, templates, screenshots, and metadata, but do not run bundled PHP, JavaScript, installers, or third-party binaries. Do not copy proprietary theme code, images, fonts, or demo content into new public skills unless the license explicitly permits it.

## Reference

Read [extraction-workflow.md](references/extraction-workflow.md) for command patterns and output formats when analyzing a theme corpus.

## Workflow

1. Inventory the corpus:
   - Count archives, extracted theme folders, plugins, images, CSS, JS, PHP, and JSON/config files.
   - Identify likely themes by `style.css`, `functions.php`, `screenshot.*`, `templates/`, `inc/`, `customizer/`, `woocommerce.php`, and Elementor template files.
2. Classify theme families:
   - Builder themes, Elementor themes, classic WP themes, ecommerce/booking themes, plugin packs, and year/version groups.
   - Domain verticals from names and metadata: agency, healthcare, education, real estate, hotel, restaurant, portfolio, shop, nonprofit, repair, industrial, event.
3. Extract design signals:
   - Header layouts, top bars, logo/nav treatments, hero/slider options, page builder templates, front-page sections, widgets, footer columns.
   - CSS selectors and recurring tokens for layout rhythm, cards, buttons, sliders, products, social icons, testimonials, portfolios, and teams.
   - Theme tags for layout support: one-column, sidebars, custom colors, featured images, WooCommerce, translation, and responsive layout.
4. Synthesize patterns:
   - Convert repeated theme structures into original design recipes.
   - Separate durable patterns from dated implementation choices such as legacy sliders, shortcodes, fixed widths, and excessive option panels.
5. Report with evidence:
   - Include counts, sample paths, representative files, and a short list of reusable lessons.
   - State any gaps caused by encrypted archives, corrupt ZIPs, missing source, or unavailable screenshots.

## Output Shape

Use this structure for findings:

- Corpus: where it was found and what was counted.
- Theme architecture: files, folders, builders, and common WordPress features.
- Visual patterns: page anatomy, sections, components, colors, typography, imagery.
- Domain patterns: differences by business vertical.
- Transferable rules: what to reuse in new frontend work.
- Avoid copying: assets/code/content that should stay out of public outputs.

## Good Extraction Questions

- What are the first-viewport patterns?
- How many header/navigation variants recur?
- Which homepage sections appear across unrelated verticals?
- Which CSS selectors reveal component priorities?
- Which theme options prove configurability that a modern frontend should expose as components or props?
- Which visual moves feel dated and should be modernized?

Prefer evidence over taste. A design lesson is stronger when you can point to several themes, a repeated file, or recurring selector patterns.
