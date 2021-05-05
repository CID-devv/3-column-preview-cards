# Frontend Mentor - 3-column preview card component solution

This is a solution to the [3-column preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/3column-preview-card-component-pH92eAR2-). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

![screenshot](./design/screenshot2.png)

### Links

- Solution URL:(https://github.com/cassandradauphin/3-column-preview-cards)
- Live Site URL:(https://3-column-preview-cards.netlify.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- SASS
- Mobile-first workflow

### What I learned

```css
.row {
  max-width: $grid-width;
  margin: 0 auto;

  @include clearfix;

  // selects all elements that start or contain class col
  [class^="col-"] {
    float: left;

    @include responsive(tab-portrait) {
      width: 100% !important;
    }
  }

  .col-1-of-3 {
    // 
    width: calc((100% - 2 * #{$gutter-horizontal}) / 3);
  }
}
```

### Continued development
- Learn more about SASS structure
- Learn more about CSS mobile 1st design 
- Learn more about CSS floats layout

### Useful resources

- [Resource 1](https://www.w3schools.com/) - This helped me for CSS float laytout. I really liked this pattern and will use it going forward.
- [Resource 2](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Floats) - This is an amazing article which helped me finally understand CSS floats. I'd recommend it to anyone still learning this concept.

## Author

- Frontend Mentor - [@cassandradauphin](https://www.frontendmentor.io/profile/cassandradauphin)
- Twitter - [@The_Haitian_Dev](https://www.twitter.com/The_Haitian_Dev)

