---
name: frontend-visual-polish
description: Review, test, and refine frontend websites, apps, dashboards, and landing pages until they feel production-ready. Use when checking responsive layout, typography, spacing, color balance, visual hierarchy, screenshots, browser behavior, interaction states, text overflow, asset rendering, or final UI quality before delivery.
---

# Frontend Visual Polish

## Goal

Make the interface look intentional at real viewport sizes. Do not stop at "it runs"; inspect the rendered UI and fix visible flaws.

## Reference

Read [qa-checklist.md](references/qa-checklist.md) when doing a thorough polish pass or when screenshots reveal layout problems.

## Polish Workflow

1. Run the app or open the page using the strongest available local method.
2. Inspect desktop and mobile widths. Add tablet if the layout has dense navigation, grids, tables, or dashboards.
3. Check first viewport:
   - The subject is immediately clear.
   - The primary action is visible.
   - The next section is hinted on both mobile and desktop for landing pages.
   - Text is not sitting inside awkwardly oversized or undersized containers.
4. Check layout stability:
   - Buttons, cards, controls, counters, boards, and fixed-format UI keep stable dimensions.
   - Text wraps cleanly and does not overlap.
   - Images crop intentionally and preserve important subject matter.
5. Check component states:
   - Hover, focus, active, disabled, selected, loading, empty, and error states are present where relevant.
   - Forms have usable labels, validation, and tap-friendly spacing.
6. Check color and typography:
   - Contrast is readable.
   - Font sizes match context.
   - Letter spacing is not negative.
   - The palette is not a one-note wash of a single hue family.
7. Fix issues directly, rerun, and reinspect.

## Screenshot Review

When browser automation is available, capture screenshots at minimum:

- Desktop: 1366x768 or similar.
- Mobile: 390x844 or similar.
- Any app-specific critical viewport, such as a wide dashboard, mobile menu open state, modal, or data-heavy page.

For canvas, Three.js, charts, generated images, or media-heavy pages, verify the rendered pixels are nonblank and correctly framed.

## Final Gate

Before final response, report:

- What was checked.
- What was changed.
- Any verification that could not be run.
- The local URL or file path if the user can preview it.
