# Product Preview Card Component

## Overview

### The challenge
Create a responsive product preview card component that:
- Displays product information clearly and attractively
- Adapts layout for mobile and desktop views
- Includes proper semantic HTML structure
- Implements accessible features
- Maintains visual consistency with the design

### Screenshot
![Product Preview Card Component](./assets/images/screenshot.png)

### Links
- [GitHub Pages](https://flaviovich.github.io/frontendmentor-challenges/product-preview-card-component/)
- [Frontend Mentor Challenge](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa)

## My Process

### Built with
- Semantic HTML5 markup
- CSS custom properties (variables)
- CSS Grid and Flexbox
- Mobile-first workflow
- Responsive images with `<picture>` element
- Accessibility features (ARIA labels, semantic structure)

### What I learned

This project helped me strengthen my skills in several areas:

**Responsive Design with Picture Element:**
```html
<picture>
  <source media="(width>= 600px)" srcset="./assets/images/image-product-desktop.jpg">
  <img class="card__image" src="./assets/images/image-product-mobile.jpg" 
       alt="Gabrielle Essence Eau De Parfum bottle surrounded by green leaves">
</picture>
```

**CSS Grid for Layout:**
```css
@media (width>=600px) {
  .card {
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-template-areas: "image body";
  }
}
```

**Accessibility Implementation:**
- Used proper semantic HTML elements (`<article>`, `<figure>`, `<section>`)
- Added ARIA labels and attributes
- Implemented proper focus states for interactive elements

**CSS Custom Properties:**
```css
:root {
  --font-montserrat: "Montserrat", sans-serif;
  --color-green-500: hsl(158, 36%, 37%);
  --spacing-md: 1.5rem;
  /* ... more variables */
}
```

### Continued development

Areas I want to continue improving:
- Advanced CSS Grid and Flexbox techniques
- More complex responsive design patterns
- JavaScript integration for interactive components
- Performance optimization for images
- Advanced accessibility features

### Useful resources

- [MDN Web Docs](https://developer.mozilla.org/) - Comprehensive web development documentation
- [CSS-Tricks](https://css-tricks.com/) - Helpful CSS techniques and guides
- [Frontend Mentor](https://www.frontendmentor.io) - Practice projects and community feedback
- [Google Fonts](https://fonts.google.com/) - Web typography resources

## Author

- Frontend Mentor - [@flaviovich](https://www.frontendmentor.io/profile/flaviovich)
- LinkedIn - [Flavio Rios](https://www.linkedin.com/in/flavio-rios-nieto/)
- [GitHub](https://github.com/flaviovich)

## Acknowledgments

Thanks to Frontend Mentor for providing this challenge that helped me practice and improve my frontend development skills. Special thanks to the developer community for sharing knowledge and best practices that made this project possible.