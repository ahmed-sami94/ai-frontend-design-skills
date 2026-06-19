# Frontend QA Checklist

Use this as the final visual gate before delivery.

## Layout

- No horizontal overflow at mobile widths.
- No clipped button text.
- No overlapping headings, cards, images, controls, or badges.
- Stable dimensions for grids, boards, product cards, stat cards, counters, and toolbars.
- Sections align to a consistent container system.
- Cards are not nested inside decorative cards.

## First Viewport

- The subject or product is obvious.
- The primary action is visible.
- The visual asset reveals the real thing, not an abstract mood.
- The next section is hinted on landing pages.
- Mobile hero height does not hide all useful content below the fold.

## Typography

- Body text is readable on mobile.
- Heading size matches the container.
- No negative letter spacing.
- Line length is comfortable.
- Long words, emails, URLs, and labels wrap or truncate intentionally.

## Color

- Text contrast is acceptable.
- Action color is distinct from passive decoration.
- The palette has neutrals, surfaces, borders, primary, accent, and status colors.
- Avoid a one-note UI dominated by one hue family unless the existing brand demands it.

## Interaction

- Links and buttons have hover/focus states.
- Form fields have labels, errors, focus, disabled, and success states where relevant.
- Navigation has active/current page state.
- Mobile menu opens, closes, and does not cover critical content awkwardly.
- Modals and dropdowns are positioned within viewport.

## Assets

- Images load.
- Important subjects are not cropped out.
- Icons match stroke/fill style.
- Empty or loading media states are handled.
- Canvas/chart/3D areas are nonblank when rendered.

## Responsive Viewports

Minimum pass:

- Mobile: around 390x844.
- Desktop: around 1366x768.

Add more when needed:

- 320px narrow mobile for tight layouts.
- Tablet for multi-column pages.
- Wide desktop for dashboards, hero framing, or data tables.

## Delivery Notes

In the final response, state verification plainly:

- Build/lint/test command if run.
- Browser/screenshot viewport if inspected.
- Any verification not run and why.
