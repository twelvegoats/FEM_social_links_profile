# Social Links Profile - Frontend Mentor Challenge

![Social Links Profile Preview](./preview.jpg)

## Overview

This project is a solution to the [Social Links Profile challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/social-links-profile-UG32l9m6dQ). It's a responsive social media profile card that showcases interactive hover states and clean design principles.

**Live Demo:** [View Live Site](https://twelvegoats.github.io/FEM_social_links_profile/)

## What I Learned

### SCSS Architecture & Organization

This project was an excellent opportunity to dive deep into **SCSS (Sass)** and learn proper CSS architecture patterns. Here's what I implemented:

#### 📁 File Structure

I organized my SCSS using a modular approach:

```
scss/
├── main.scss           # Main entry point
├── utils/
│   └── _variables.scss # Color palette, typography, spacing
├── base/
│   ├── _resets.scss   # CSS resets
│   └── _base.scss     # Base component styles
```

#### 🎨 SCSS Variables

I learned to create a comprehensive design system using SCSS variables:

```scss
// Color System
$green: hsl(75, 94%, 57%);
$white: hsl(0, 0%, 100%);
$grey-700: hsl(0, 0%, 20%);
$grey-800: hsl(0, 0%, 12%);
$grey-900: hsl(0, 0%, 8%);

// Typography Scale
$body-copy: 0.875rem;
$font-family: 'Inter', sans-serif;
$font-weight-regular: 400;
$font-weight-semibold: 600;
$font-weight-bold: 700;

// Consistent Spacing
$spacing-small: 0.5rem;
$spacing-medium: 1rem;
$spacing-large: 1.5rem;
```

#### 🔧 SCSS Features Utilized

1. Partials & Imports: Used `@use` directive for better module management
2. Variables: Created a consistent design token system
3. Nesting: Organized related styles hierarchically
4. Mixins: (Future enhancement opportunity)
5. Functions: (Future enhancement opportunity)

### CSS Techniques Mastered

#### Flexbox Layout

```
.social-card {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.social-card__links {
  display: flex;
  flex-direction: column;
  width: 100%;
}
```

#### Interactive States

```
.social-card__link {
  transition: background-color 0.3s ease;

  &:hover {
    background-color: $green;
    color: $grey-900;
  }
}
```

#### BEM Methodology

I implemented BEM (Block Element Modifier) naming convention:

- Block: `.social-card`
- Elements: `.social-card__name`, `.social-card__link`, `.social-card__bio`
- Modifiers: (Used for state variations)

### Responsive Design Principles

- Mobile-first approach
- Flexible units (rem, %)
- Proper viewport meta tag
- Scalable typography

### Accessibility Considerations

- Semantic HTML structure
- Proper alt text for images
- Focus states for interactive elements
- Color contrast compliance

## Technologies Used

- HTML5: Semantic markup
- SCSS/Sass: CSS preprocessing
- CSS3: Modern styling techniques

## Key Features

- ✅ Responsive design that works on all devices
- ✅ Interactive hover states with smooth transitions
- ✅ Clean, modern design following the provided mockups
- ✅ Accessible markup and styling
- ✅ Organized SCSS architecture

## Lessons Learned

### SCSS Benefits I Discovered:

1.  Better Organization: Splitting styles into logical partials made the codebase much more maintainable
2.  Design Consistency: Variables ensured consistent spacing, colors, and typography throughout
3.  Scalability: The modular structure makes it easy to add new components
4.  Developer Experience: Features like nesting and variables made writing CSS more enjoyable

### Areas for Future Improvement:

- Implement SCSS mixins for repeated patterns
- Add CSS custom properties for runtime theming
- Explore SCSS functions for dynamic calculations
- Add more sophisticated responsive breakpoint management

## Author

**Sean Wildman**

GitHub: [@twelvegoats](https://github.com/twelvegoats)

Frontend Mentor: [@twelvegoats](https://www.frontendmentor.io/profile/twelvegoats)

## Acknowledgments

- Challenge by [Frontend Mentor](https://www.frontendmentor.io/)

_This project represents my journey in learning SCSS and modern CSS architecture. Each commit shows progression in understanding modular CSS and design system thinking._
