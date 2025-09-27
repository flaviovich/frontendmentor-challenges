# Frontend Mentor - Stats preview card component solution

This is a solution to the [Stats preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/stats-preview-card-component-8JqbgoU62). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![Desktop View](./assets/images/screenshot.png)

### Links

- Live Site URL: [GitHub Pages](https://flaviovich.github.io/frontendmentor-challenges/stats-preview-card-component/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties (CSS variables)
- Flexbox
- Mobile-first workflow
- Responsive images with `<picture>` element
- CSS Grid for statistics layout
- Modern CSS features:
  - `font-variation-settings` for Inter font
  - `mix-blend-mode` for image overlay effect
  - `dvh` units for better mobile viewport handling

### What I learned

This project helped me reinforce several key concepts:

**Responsive Images:**
```html
<picture class="card__picture">
  <source media="(min-width: 1024px)" srcset="./assets/images/image-header-desktop.jpg">
  <img class="card__image" src="./assets/images/image-header-mobile.jpg"
    alt="Team of professionals working together in a modern office environment with data analytics on screens">
</picture>
```

**CSS Mix Blend Mode for Image Overlays:**
```css
.card__picture::before {
  content: "";
  position: absolute;
  background-color: var(--color-purple-500);
  mix-blend-mode: multiply;
  opacity: 0.75;
}
```

**Semantic HTML for Statistics:**
```html
<dl>
  <div class="stats__item">
    <dt class="stats__label">Companies</dt>
    <dd class="stats__value">10k+</dd>
  </div>
</dl>
```

**CSS Custom Properties for Consistent Design:**
```css
:root {
  --color-navy-950: hsl(233, 47%, 7%);
  --color-purple-500: hsl(277, 64%, 61%);
  --font-inter: "Inter", sans-serif;
}
```

### Continued development

Areas I want to continue focusing on in future projects:

- **Advanced CSS Grid layouts** - Exploring more complex grid patterns
- **CSS Container Queries** - For more component-based responsive design
- **Web Performance Optimization** - Image optimization and loading strategies
- **Accessibility improvements** - Better screen reader support and keyboard navigation
- **CSS animations and transitions** - Adding subtle micro-interactions

### Useful resources

- [MDN Web Docs - mix-blend-mode](https://developer.mozilla.org/en-US/docs/Web/CSS/mix-blend-mode) - Excellent resource for understanding blend modes
- [CSS-Tricks - A Complete Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) - Always helpful for flexbox layouts
- [Web.dev - Responsive Images](https://web.dev/responsive-images/) - Great guide for implementing responsive images
- [Modern CSS Solutions](https://moderncss.dev/) - Helped with modern CSS techniques and best practices
- [Can I Use](https://caniuse.com/) - Essential for checking browser compatibility

## Author

- Linkedin - [Flavio Rios](https://www.linkedin.com/in/flavio-rios-nieto/)
- Frontend Mentor - [@flaviovich](https://www.frontendmentor.io/profile/flaviovich)

## Acknowledgments

Thanks to Frontend Mentor for providing this challenge and to the community for their feedback and inspiration. Special appreciation for the detailed design files and style guide that made this implementation possible.

The challenge helped me practice responsive design principles and modern CSS techniques, particularly working with image overlays and responsive images using the `<picture>` element.