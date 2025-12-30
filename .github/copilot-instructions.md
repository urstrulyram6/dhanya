# Dhanya Tea House Website - AI Coding Guidelines

## Project Overview
This is a static website template for a tea house/shop, built with Bootstrap 5. It features multiple HTML pages (home, about, products, etc.) with responsive design, animations, and interactive elements.

## Architecture
- **Static Site**: No backend or build process; serves HTML/CSS/JS directly
- **Page Structure**: Each `.html` file in root is a complete page with embedded styles/scripts
- **Assets**: 
  - `css/style.css`: Custom styles with CSS variables for theming
  - `js/main.js`: jQuery-based interactions (carousels, animations, modals)
  - `lib/`: Third-party libraries (Bootstrap, Owl Carousel, Wow.js, etc.)
  - `img/`: Static images
  - `scss/`: Bootstrap source (not compiled; use pre-built `css/bootstrap.min.css`)

## Key Patterns
- **HTML Structure**: Bootstrap grid system (`container`, `row`, `col-*`) with sections like `section-title`, `wow fadeIn` animations
- **Navigation**: Sticky navbar with dropdowns; update `navbarCollapse` links for new pages
- **Carousels**: Owl Carousel for products/testimonials; configured in `main.js`
- **Animations**: Wow.js with `data-wow-delay` for scroll-triggered effects
- **Modals**: Bootstrap modals for videos/contact; JS handles dynamic content
- **Colors**: Use CSS variables (`--primary: #88B44E`, `--secondary: #FB9F38`) for consistency

## Conventions
- **File Naming**: Kebab-case (e.g., `about.html`, `style.css`)
- **Classes**: Bootstrap classes first, then custom (e.g., `btn btn-primary rounded-pill`)
- **Images**: Place in `img/`; reference as `img/filename.jpg`
- **Links**: Relative paths; update navbar for new pages
- **Responsive**: Mobile-first with Bootstrap breakpoints

## Adding Features
- **New Page**: Copy `index.html`, change content, add to navbar
- **New Section**: Use existing structure (e.g., `<div class="container-xxl py-5">` with `section-title`)
- **Styling**: Add to `css/style.css`; use variables for colors
- **JS**: Extend `js/main.js` with jQuery; initialize plugins after DOM ready
- **Images**: Add to `img/`; optimize for web

## Common Tasks
- Update content: Edit HTML directly
- Change theme: Modify CSS variables in `:root`
- Add carousel: Use `.owl-carousel` class; configure in JS
- Animate elements: Add `wow` class and `data-wow-delay`

## Dependencies
- Bootstrap 5.0.0 (CDN + local)
- jQuery 3.6.1
- Font Awesome 5.10.0
- Google Fonts: Open Sans, Playfair Display

Avoid modifying `lib/` or `scss/` unless customizing Bootstrap.</content>
<parameter name="filePath">e:\Shanu\dhanya\.github\copilot-instructions.md