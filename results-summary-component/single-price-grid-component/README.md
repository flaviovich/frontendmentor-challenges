# Single Price Grid Component

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

- View the optimal layout for the component depending on their device's screen size
- See a hover state on desktop for the Sign Up call-to-action

### Screenshot

![Desktop Design](./assets/images/screenshot.png)

### Links

- [Solution URL](https://github.com/flaviovich/frontendmentor-challenges/tree/main/single-price-grid-component)
- [Live Site URL](https://codepen.io/flaviovich/pen/WbQBddw?editors=1100)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- CSS Grid
- CSS Flexbox
- Mobile-first workflow
- Responsive design principles

### What I learned

This project was an excellent opportunity to deepen my understanding of CSS Grid layout and responsive design patterns. Here are some key takeaways:

**CSS Grid Implementation:**
```css
/* Mobile-first single column layout */
.container {
  display: grid;
  grid-template-columns: 1fr;
  grid-template-rows: auto auto auto;
}

/* Desktop layout using grid-template-areas */
@media (width > 1024px) {
  .container {
    grid-template-columns: 1fr 1fr;
    grid-template-rows: auto auto;
    grid-template-areas:
      "intro intro"
      "plan features";
    max-width: 700px;
  }
  
  .intro { grid-area: intro; }
  .plan { grid-area: plan; }
  .features { grid-area: features; }
}
```

**Color Management with CSS Variables:**
```css
:root {
  --color-teal-500: hsl(179, 62%, 43%);
  --color-green-400: hsl(71, 73%, 54%);
  --color-slate-100: hsl(204, 43%, 93%);
  --color-gray-500: hsl(218, 22%, 67%);
}
```

**Responsive Typography and Spacing:**
```css
/* Mobile padding */
.intro, .plan, .features {
  padding: 2rem 1.5rem;
}

/* Desktop padding */
@media (width > 1024px) {
  .intro, .plan, .features {
    padding: 2.5rem;
  }
}
```

### Continued development

Areas I want to continue focusing on in future projects:

- **Advanced CSS Grid techniques**: Exploring more complex grid layouts and subgrid
- **CSS Architecture**: Improving my approach to organizing and scaling CSS codebases
- **Accessibility**: Enhancing focus states and screen reader compatibility
- **Performance Optimization**: Reducing CSS bundle size and improving rendering performance
- **Cross-browser Compatibility**: Testing and ensuring consistent experiences across all browsers

### Useful resources

- [CSS Grid Guide](https://css-tricks.com/snippets/css/complete-guide-grid/) - Comprehensive guide to CSS Grid layout
- [Flexbox Guide](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) - Excellent Flexbox reference
- [Color Contrast Checker](https://webaim.org/resources/contrastchecker/) - Essential for accessibility testing
- [Google Fonts](https://fonts.google.com/) - For typography management

## Author

- Website - [Flavio Rios](https://www.linkedin.com/in/flavio-rios-nieto/)
- Frontend Mentor - [@flaviovich](https://www.frontendmentor.io/profile/flaviovich)
- Twitter - [@flaviovichDev](https://www.twitter.com/flaviovichDev)

## Acknowledgments

I'd like to thank the Frontend Mentor community for providing this challenge and the valuable feedback from other developers. Special thanks to:

- The CSS-Tricks team for their comprehensive guides on Grid and Flexbox
- The Google Fonts team for providing excellent typography options
- The web development community for sharing knowledge and best practices