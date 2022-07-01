# Frontend Mentor - Product preview card component solution

[Live Preview](https://golden-dolphin-05dcd8.netlify.app/)

This is a solution to the [Product preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa).

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

### Screenshot

![](./screenshot.jpg)

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [https://golden-dolphin-05dcd8.netlify.app/](https://golden-dolphin-05dcd8.netlify.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow
- CUBE CSS methodology

### What I learned

I used this as a simple project to explore [CUBE CSS](https://cube.fyi/). Specifically in this project I've used fluid typography and space scales to keep a visual rhythm and have subtly bigger text on larger screens.

I had attempted to use the principles of intrinsic design, and avoid media queries. However, that conflicts with using the `<picture>` element for art direction. The picture element needs a media query to know when to serve which aspect ratio of image. To avoid this happening at a different point to the layout changing from vertical to horizontal, I had to use a media query with the same breakpoint for both. This makes the implementation less resiliant to how the component would be used within the page. However, I don't see any way around this. Even container queries wouldn't solve the `<picture>` issue.

I've used a lot of CSS custom properties here. One use I particularly like is for setting up default transition properties. This allowed me to override just the motion animation for users with `prefers-reduced-motion`. Many CSS resets switch off all animations in this case, but here this still allows opacity and color changes to have transitions, giving a more elegant result.

### Useful resources

- [CUBE CSS](https://cube.fyi/) - I followed the broad ideas of CUBE to keep the CSS organized.
- [Utopia](https://utopia.fyi/) - I used Utopia to generate the fluid size and spacing scales.

## Author

- Github - [Alex Marshall](https://github.com/AlexKMarshall)
- Frontend Mentor - [@AlexKMarshall](https://www.frontendmentor.io/profile/AlexKMarshall)
- Twitter - [@AlexKMarshall1](https://twitter.com/alexkmarshall1)
