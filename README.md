# Bridal7Groom SA Website

This is my website project for Bridal7Groom SA, a nonprofit that helps couples in South Africa plan affordable weddings. It's for my web development module assignment.

## What This Is

Basically a responsive website built with HTML, CSS, and JavaScript. No fancy frameworks or build tools - you can just open the HTML file in your browser and it should work. I used Tailwind CSS from CDN for some styling help but mostly wrote my own CSS.

## Files

- `POE.html` - the main HTML file with all the content
- `Style.css` - all my custom CSS styles
- `script.js` - JavaScript for the menu, forms, and interactive stuff
- `README.md` - this file

## Features

I added:
- Responsive design that works on mobile, tablet, and desktop
- Mobile menu that toggles properly
- Contact form with validation (checks email format, name length, etc.)
- Smooth scrolling when you click nav links
- Accessibility features like ARIA labels and keyboard navigation
- Newsletter signup in the footer
- Gallery with lightbox for viewing images
- Search functionality to find content
- Interactive map in the contact section

## Setup

Just open `POE.html` in any modern browser. That's it.

Note: The site uses CDN links for Tailwind CSS, Font Awesome icons, and Google Fonts, so you need internet for everything to load properly.

## How It Works

### JavaScript (script.js)

I wrote JavaScript to handle:
- Mobile menu toggle (opens/closes when you click the hamburger icon)
- Smooth scrolling when clicking navigation links
- Form validation for the contact form
- Email validation using regex pattern
- Character counter for the message field (shows 0/1000)
- Newsletter form submission
- Keyboard shortcuts (ESC closes mobile menu)
- Auto-closes mobile menu when window resizes to desktop size
- Gallery lightbox for viewing images in full size
- Search functionality that filters content

I wrapped everything in an IIFE (Immediately Invoked Function Expression) so it doesn't pollute the global scope. Learned that from MDN docs.

### CSS (Style.css)

My CSS includes:
- Custom CSS variables for colors (makes it easier to change colors later)
- Responsive breakpoints using media queries for different screen sizes
- Hover effects and transitions for buttons and cards
- Focus styles for accessibility (visible outlines when tabbing)
- Print styles (hides navigation and buttons when printing)
- Reduced motion support for users who prefer less animation

I mixed my custom CSS with Tailwind utility classes from the CDN. Tailwind helped with spacing and layout stuff.

### HTML (POE.html)

I used semantic HTML5 elements:
- Proper heading hierarchy (h1, h2, h3)
- ARIA labels where needed for screen readers
- Skip to content link for keyboard users
- Form labels and error messages
- Figure and figcaption for images
- Meta keywords and description for SEO

## Form Validation

The contact form validates:
- Name must be at least 2 characters
- Email must be valid format (checks for @ and domain)
- Subject must be selected from dropdown
- Message must be at least 10 characters (max 1000)

Errors show up in real-time as you type or when you leave a field. I added proper ARIA attributes so screen readers can announce the errors.

## Browser Support

I tested it in:
- Chrome (works great)
- Firefox (works fine)
- Safari (should work, didn't test extensively)
- Edge (works)

Didn't test in IE11 and probably won't work there, but who uses that anymore?

## Accessibility

I tried to make it accessible:
- ARIA labels on buttons and links
- Keyboard navigation works throughout
- Focus management when sections are focused
- Screen reader friendly structure
- Skip link for keyboard users
- Reduced motion support

I followed WCAG guidelines as much as I could for a static site without a backend.

## Notes

- Images are hosted externally (Google Cloud Storage URLs) - not ideal but works for now
- Forms don't actually submit anywhere - would need a backend server for that
- Tailwind CSS loads from CDN (just using utilities, not the full framework)
- Font Awesome for icons
- Google Fonts for typography (Playfair Display and Inter)

## Changelog

### Version 1.0 - Final Submission (2024)

**Added Features:**
- Added interactive Google Maps embed in contact section
- Implemented gallery lightbox functionality for viewing images
- Added search functionality to find content across the site
- Added meta keywords for SEO optimization
- Enhanced navigation with Gallery link

**Improvements:**
- Improved form validation with better error messages
- Added keyboard navigation support for lightbox (arrow keys, ESC)
- Enhanced mobile menu functionality
- Better responsive design for tablet sizes

**Bug Fixes:**
- Fixed mobile menu not closing when clicking nav links
- Fixed form validation not clearing errors properly
- Improved focus management for accessibility

### Initial Development

**Part 1:**
- Created basic HTML structure with semantic elements
- Added navigation menu with smooth scrolling
- Implemented responsive design with media queries
- Added contact form with basic validation
- Created services section with images
- Added success stories/testimonials section
- Implemented donation section
- Added footer with newsletter signup

**Part 2:**
- Created external CSS stylesheet
- Added CSS variables for theming
- Implemented responsive breakpoints for mobile, tablet, desktop
- Added hover effects and transitions
- Implemented print styles
- Added accessibility features (focus styles, ARIA labels)
- Enhanced form validation with real-time feedback

**Part 3:**
- Added interactive elements (lightbox, search, map)
- Enhanced form functionality
- Added SEO meta tags
- Improved overall user experience

## References

### Documentation & Learning Resources

**MDN Web Docs:**
- MDN Web Docs - CSS. (n.d.). *CSS: Cascading Style Sheets*. Mozilla Developer Network. https://developer.mozilla.org/en-US/docs/Web/CSS
- MDN Web Docs - JavaScript. (n.d.). *JavaScript*. Mozilla Developer Network. https://developer.mozilla.org/en-US/docs/Web/JavaScript
- MDN Web Docs - HTML. (n.d.). *HTML: HyperText Markup Language*. Mozilla Developer Network. https://developer.mozilla.org/en-US/docs/Web/HTML
- MDN Web Docs - ARIA. (n.d.). *Accessible Rich Internet Applications (ARIA)*. Mozilla Developer Network. https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA

**CSS Resources:**
- MDN Web Docs. (n.d.). *Using CSS custom properties (variables)*. https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties
- MDN Web Docs. (n.d.). *Using media queries*. https://developer.mozilla.org/en-US/docs/Web/CSS/Media_Queries
- MDN Web Docs. (n.d.). *Using CSS transitions*. https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Transitions
- CSS-Tricks. (n.d.). *A Complete Guide to Flexbox*. https://css-tricks.com/snippets/css/a-guide-to-flexbox/
- CSS-Tricks. (n.d.). *A Complete Guide to Grid*. https://css-tricks.com/snippets/css/complete-guide-grid/

**JavaScript Resources:**
- MDN Web Docs. (n.d.). *Document Object Model (DOM)*. https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model
- MDN Web Docs. (n.d.). *EventTarget.addEventListener()*. https://developer.mozilla.org/en-US/docs/Web/API/EventTarget/addEventListener
- MDN Web Docs. (n.d.). *Client-side form validation*. https://developer.mozilla.org/en-US/docs/Learn/Forms/Form_validation
- MDN Web Docs. (n.d.). *Regular expressions*. https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions

### Accessibility Resources

- W3C. (n.d.). *WCAG 2.1 Quick Reference*. Web Accessibility Initiative. https://www.w3.org/WAI/WCAG21/quickref/
- WebAIM. (n.d.). *Web Accessibility In Mind*. https://webaim.org/
- The A11y Project. (n.d.). *The A11y Project - A community-driven effort to make web accessibility easier*. https://www.a11yproject.com/
- W3C. (n.d.). *WAI-ARIA Authoring Practices Guide*. https://www.w3.org/WAI/ARIA/apg/
- MDN Web Docs. (n.d.). *ARIA labels and relationships*. https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes

### External Libraries & Tools

**CSS Frameworks:**
- Tailwind Labs. (n.d.). *Tailwind CSS - Rapidly build modern websites*. https://tailwindcss.com/
- Tailwind CSS CDN. (n.d.). *Tailwind CSS Play CDN*. https://cdn.tailwindcss.com/

**Icons:**
- Font Awesome. (n.d.). *Font Awesome - The Internet's Icon Library*. https://fontawesome.com/
- Font Awesome CDN. (n.d.). *Font Awesome 6.0.0 via CDNJS*. https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css

**Typography:**
- Google Fonts. (n.d.). *Google Fonts - Making the web more beautiful, fast, and open*. https://fonts.google.com/

### Web Standards & Best Practices

- W3C. (n.d.). *HTML Living Standard*. https://html.spec.whatwg.org/
- W3C. (n.d.). *CSS Specifications*. https://www.w3.org/Style/CSS/
- W3C. (n.d.). *ECMAScript Language Specification*. https://tc39.es/ecma262/
- Google Developers. (n.d.). *Web Fundamentals*. https://developers.google.com/web/fundamentals
- Web.dev. (n.d.). *Learn web development*. https://web.dev/

### Responsive Design

- MDN Web Docs. (n.d.). *Responsive design*. https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Responsive_Design
- Google Developers. (n.d.). *Responsive Web Design Basics*. https://developers.google.com/web/fundamentals/design-and-ux/responsive

### Form Validation & UX

- MDN Web Docs. (n.d.). *HTML5 form validation*. https://developer.mozilla.org/en-US/docs/Learn/Forms/Form_validation
- Nielsen Norman Group. (n.d.). *Usability Guidelines*. https://www.nngroup.com/articles/

## License

This is for educational purposes only. The content belongs to Bridal7Groom SA (fictional organization for assignment purposes).

## Contact

If you have questions about the code or want to reach out, use the contact form on the website.

---

Last updated: November 2025
