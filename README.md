# Summit Consulting Website

A modern replica of the Summit Consulting website built with Vue 3 and Tailwind CSS, featuring a clean black and white design with customizable color variables.

## Features

- **Responsive Design**: Mobile-first approach with responsive layouts
- **Modern Vue 3**: Built with Composition API and reactive components
- **Tailwind CSS**: Utility-first CSS framework for rapid styling
- **Customizable Colors**: CSS variables for primary, accent, and background colors
- **Interactive Components**: Mobile navigation, contact forms, and hover effects
- **Accessibility**: Semantic HTML and proper ARIA labels

## Color Variables

The website uses CSS custom properties for easy color customization:

```css
:root {
  --color-primary: #000000;    /* Main text and accent color */
  --color-accent: #666666;     /* Secondary text and borders */
  --color-background: #ffffff; /* Background color */
}
```

## Project Structure

```
src/
├── components/
│   ├── Header.vue           # Navigation header
│   ├── HeroSection.vue      # Main hero section
│   ├── ServicesSection.vue  # Services overview
│   ├── TestimonialsSection.vue # Client testimonials
│   ├── BlogSection.vue      # Blog/news section
│   ├── ContactSection.vue   # Contact form and info
│   └── Footer.vue           # Site footer
├── App.vue                  # Main app component
├── main.js                  # Vue app entry point
└── style.css               # Global styles and Tailwind imports
```

## Installation

1. Install dependencies:
```bash
npm install
```

2. Start development server:
```bash
npm run dev
```

3. Build for production:
```bash
npm run build
```

## Sections

- **Header**: Responsive navigation with mobile menu
- **Hero**: Main heading with services overview
- **Services**: Marketing, Business, and Events service cards
- **Testimonials**: Client reviews and feedback
- **Blog**: Latest articles and news
- **Contact**: Contact form and company information
- **Footer**: Links, contact info, and newsletter signup

## Customization

To change colors, modify the CSS variables in `src/style.css`:

```css
:root {
  --color-primary: #your-primary-color;
  --color-accent: #your-accent-color;
  --color-background: #your-background-color;
}
```

## Technologies Used

- Vue 3 with Composition API
- Tailwind CSS
- Vite (build tool)
- PostCSS
- Autoprefixer

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
