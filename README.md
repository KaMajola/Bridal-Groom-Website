# Bridal7Groom SA — Part 2 CSS Styling and Responsive Design

This project implements an accessible, responsive, and visually cohesive single-page website for the nonprofit Bridal7Groom SA. It addresses Part 2 requirements: external stylesheet, base styles, typography, layout, decoration/colour, responsive breakpoints, images, and documentation.

## How to run
Open `Index.html` in a modern browser. No build step is required.

## Stylesheet
- External stylesheet: `Style.css` is linked from `Index.html`.
- Uses a CSS reset via universal selector and establishes typography scales with Google Fonts (`Inter`, `Playfair Display`).
- Includes selectors: universal, element, class, id, attribute, descendant, pseudo-class, and pseudo-element.
- Layout uses modern CSS Grid/Flexbox (via utility classes from Tailwind CDN in HTML and custom classes in CSS).

## Responsiveness
- Breakpoints: 1024px (desktop), 768px (tablet), 640px (mobile).
- Adjusts spacing, grids, navigation visibility, and forms for each breakpoint.
- Uses relative units (`rem`, `%`) and responsive images via `picture`, `sizes`, and `loading="lazy"`.

## Accessibility
- Semantic landmarks: `main`, `nav`, `section`, `figure`, `footer`.
- `aria-labelledby` references and descriptive `alt` text.
- Focus-visible styles for keyboard navigation.

## Changelog
- 2025-09-19: Standardised stylesheet link to `Style.css`. Added semantic `main` landmark, responsive `picture` in hero, `loading="lazy"` on gallery images. Fixed list markup errors in Services and Community sections. Added nav underline pseudo-element effect, base CSS variables, accessibility focus styles, and print styles. Created this README with rubric mapping.
- 2025-09-19: Improved mobile/tablet layouts: stacked grids, spacing tweaks, contact info stacking, larger touch targets.

## References
- Font Awesome 6 CDN for icons (`https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css`).
- Google Fonts: Inter, Playfair Display.
- Tailwind CSS CDN for utility classes (used for layout and spacing only).
