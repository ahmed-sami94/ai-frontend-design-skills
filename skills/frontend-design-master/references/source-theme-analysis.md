# Source Theme Analysis

This reference summarizes the theme corpus that inspired the skill. It records transferable frontend lessons only. Do not copy original theme code, images, demo content, fonts, or bundled plugins into public outputs.

## Corpus Snapshot

Public summary: `372 website/theme packages analyzed`.

- 372 ZIP packages reviewed.
- 353 theme-like ZIPs with both `style.css` and `functions.php`.
- 356 ZIPs with `style.css`.
- 342 ZIPs mentioning Customizer files.
- 342 ZIPs mentioning WooCommerce.
- 41 ZIPs mentioning Elementor or builder-style files.
- Main package groups: yearly theme groups, builder theme groups, Elementor-style theme groups, other theme groups, and plugin groups.

Representative repeated files:

- `customizer/controls/settings-frontpage.php`
- `customizer/controls/settings-header.php`
- `customizer/controls/settings-footer.php`
- `frontpage/slider.php`
- `frontpage/slider-static.php`
- `frontpage/slider-customslider.php`
- `templates/head-type1.php` through `head-type4.php`
- `templates/contact-layout1.php`
- `templates/contact-layout2.php`
- `templates/page-builder.php`
- `templates/blog_template.php`
- `woocommerce.php`

Recurring selector patterns from sampled CSS:

- ecommerce selectors for product cards, carts, product lists, and shop pages.
- header selectors for logos, contact strips, navigation, and utility areas.
- slider selectors for hero images, captions, and vertical slider layouts.
- CTA selectors for buttons and read-more actions.
- social selectors for icons and sharing links.
- testimonial, team, portfolio, gallery, and footer-column selectors.

Common theme tags:

- `custom-menu`, `theme-options`, `right-sidebar`, `featured-images`, `threaded-comments`
- `custom-background`, `custom-header`, `sticky-post`, `one-column`
- `custom-colors`, `flexible-header`, `full-width-template`, `two-columns`
- `translation-ready`, `responsive-layout`, `e-commerce`, `portfolio`

## Transferable Lessons

Commercial WordPress themes usually sell configurability. Modern frontend work should translate that into clear component variants rather than huge option panels.

1. Header variants are core architecture, not decoration:
   - Top contact strip.
   - Logo plus tagline.
   - Primary navigation.
   - Social links or utility actions.
   - Sticky or compact variants.
2. Hero modules need content and behavior choices:
   - Static hero.
   - Slider or carousel.
   - No hero for dense app/dashboard flows.
   - Caption title, description, and one or two CTAs.
3. Front pages are section systems:
   - Services, features, portfolio, team, testimonials, blog/news, contact, product/shop, and footer widgets.
4. Domain themes mostly change evidence and imagery, not page logic:
   - Healthcare needs trust, departments, doctors, appointments.
   - Education needs courses, outcomes, events, admissions.
   - Real estate needs listings, filters, location, agent proof.
   - Restaurant/hotel needs menus, rooms, booking, ambience, reviews.
   - Agency/software needs capability proof, case studies, process, conversion.
5. Ecommerce readiness affects many surfaces:
   - Product cards, category grids, cart affordances, price states, sale labels, and checkout confidence cues.
6. The dated parts should be modernized:
   - Legacy slider effects, crowded top bars, small typography, excessive columns, generic stock images, and shortcode-heavy content.

## Design Translation

When creating a fresh frontend inspired by this corpus:

- Convert front-page option files into component props or content config.
- Convert multiple header template files into a small header variant API.
- Convert widget areas into reusable layout slots.
- Convert ecommerce selectors into modern product/card states.
- Convert section button settings into a consistent CTA component.
- Convert old sidebar-heavy templates into responsive content layouts.

Keep the lesson; rewrite the implementation.
