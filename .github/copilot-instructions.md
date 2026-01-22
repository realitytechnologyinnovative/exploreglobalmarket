# Techex Template - AI Coding Guidelines

## Project Overview
This is a static HTML template for a technology/IT services website. It consists of multiple HTML pages with shared assets (CSS, JS, images). No build system or backend - all files are served directly.

## File Structure
- **Root HTML files**: `index.html`, `about.html`, etc. - individual pages
- **Assets**: `assets/css/`, `assets/js/`, `assets/images/`, `assets/fonts/`
- **Key files**:
  - `assets/css/style.css`: Main custom styles with sectioned comments
  - `assets/js/custom.js`: jQuery-based interactions and Owl Carousel configurations
  - `assets/css/responsive.css`: Mobile/tablet styles
  - `assets/css/theme-dark.css`: Dark theme overrides

## Development Patterns
- **HTML Structure**: Uses Bootstrap grid system with custom classes like `pt-100`, `pb-70` for spacing
- **CSS Organization**: Styles are grouped by component in `style.css` (e.g., "Main Banner Area Style", "Services Area Style")
- **JavaScript**: jQuery plugins for navigation (meanmenu), sliders (owlCarousel), and interactions
- **Images**: Organized by feature in `assets/images/` subfolders (e.g., `home-one/`, `services/`, `team/`)
- **Icons**: Flaticon font icons via `assets/fonts/flaticon.css` and Boxicons via CDN

## Common Tasks
- **Adding a new page**: Copy an existing HTML file, update navigation links in all pages
- **Styling components**: Add styles to `style.css` under appropriate section comment, or create new section
- **Responsive design**: Use Bootstrap breakpoints + custom media queries in `responsive.css`
- **Dark theme**: Override light styles in `theme-dark.css` using `.theme-dark` class
- **Sliders/Carousels**: Configure in `custom.js` using Owl Carousel options (see existing `.owlCarousel()` calls)

## Key Conventions
- **Class naming**: Bootstrap classes + custom descriptive names (e.g., `banner-slider`, `case-study-slider`)
- **Spacing**: Consistent padding/margin classes like `ptb-100` (padding top/bottom 100px)
- **Color scheme**: Primary colors defined in `:root` variables in `style.css`
- **Navigation**: Multi-level dropdowns using Bootstrap nav with custom hover effects

## External Dependencies
- **Bootstrap 5**: Layout and components
- **jQuery**: DOM manipulation and plugins
- **Owl Carousel**: Image/content sliders
- **Boxicons**: Icon library
- **Google Fonts**: Livvic font family

## Deployment
Static files - deploy by uploading entire directory to web server. No compilation required.