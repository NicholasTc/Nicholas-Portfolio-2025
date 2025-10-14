# Portfolio Website - Astro Implementation

A modern, responsive portfolio website built with Astro, featuring a clean design with dark/light theme toggle, project filtering, and interactive modals.

## Features

- **Modern Design**: Clean, minimalist design with dark/light theme support
- **Responsive Layout**: Fully responsive across all device sizes
- **Project Filtering**: Filter projects by technology stack (Web, Backend, ML, WordPress)
- **Interactive Modals**: Quick-view modals for project details
- **Theme Toggle**: Switch between dark and light themes with system preference detection
- **Smooth Animations**: Button hover effects, ripple animations, and smooth transitions
- **Accessibility**: ARIA labels, keyboard navigation, and screen reader support

## Project Structure

```
src/
├── layouts/
│   └── BaseLayout.astro    # Main layout with navigation and theme toggle
├── pages/
│   └── index.astro         # Home page with projects and modals
└── components/             # Reusable components (to be added)

public/
└── favicon.svg            # Site favicon

PreviewPages/              # Original HTML previews for reference
├── homePreview.html
└── modalPreview.html
```

## Getting Started

1. **Install dependencies**:

   ```bash
   npm install
   ```

2. **Start development server**:

   ```bash
   npm run dev
   ```

3. **Build for production**:

   ```bash
   npm run build
   ```

4. **Preview production build**:
   ```bash
   npm run preview
   ```

## Development

The website is built with Astro and uses:

- **CSS Custom Properties** for theming and design tokens
- **Vanilla JavaScript** for interactions (theme toggle, filtering, modals)
- **Responsive Design** with CSS Grid and Flexbox
- **Modern CSS Features** like `color-mix()`, backdrop filters, and CSS animations

## Customization

### Theme Colors

Edit the CSS custom properties in `BaseLayout.astro` to customize the color scheme:

```css
:root {
  --bg: #0b0f17; /* Background color */
  --surface: #0f172a; /* Surface/card color */
  --text: #e5e7eb; /* Text color */
  --accent: #60a5fa; /* Accent color */
  /* ... more variables */
}
```

### Content

- Update personal information in `index.astro`
- Replace placeholder images with your own project screenshots
- Modify project data and descriptions
- Add your own contact information

### Projects

Add new projects by duplicating the existing project card structure and updating:

- Project title and description
- Technology badges
- Impact metrics
- Modal content for quick-view details

## Browser Support

- Chrome 88+
- Firefox 87+
- Safari 14+
- Edge 88+

## License

This project is open source and available under the MIT License.
