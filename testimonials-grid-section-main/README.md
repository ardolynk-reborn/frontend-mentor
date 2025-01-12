# Frontend Mentor - Testimonials grid section solution

This is a solution to the [Testimonials grid section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/testimonials-grid-section-Nnw6J7Un7). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size

### Screenshot

![](./screenshot.jpg)

### Links

- Solution URL: [Testimonials grid section source code](https://github.com/ardolynk-reborn/frontend-mentor/tree/main/testimonials-grid-section-main)
- Live Site URL: [Testimonials grid section live](https://ardolynk-reborn.github.io/frontend-mentor/testimonials-grid-section-main)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow
- [SASS](https://sass-lang.com/) - CSS preprocessor

### What I learned

Here we'd better use a grid with fixed percentage per row / column. Also for this solution I finally used SASS preprocessor.

```sass
@mixin desktop
  @media (min-width: 48em)
    @content

main
  padding: 48px 0 48px 0
  max-width: 70em

  @include desktop
    display: grid
    grid-template-columns: repeat(4, 25%)
    grid-template-rows: repeat(2, 50%)
```

Another complexity connected with a background of the first card. Here I defined `background: url(./images/bg-pattern-quotation.svg) no-repeat 90% 0 hsl(263, 55%, 52%)`.

### Continued development

I would like to design my landing page.

### Useful resources

- [Media Query Breakpoints with SASS](https://dev.to/serifcolakel/breakpoints-with-sass-in-react-2k59) - This article helps to use media breakpoints in SASS more effectively.

## Author

- GitHub - [@ardolynk-reborn](https://github.com/ardolynk-reborn)
- Frontend Mentor - [@ardolynk-reborn](https://www.frontendmentor.io/profile/ardolynk-reborn)
- Twitter - [@ardolynk75](https://x.com/ardolynk75)
