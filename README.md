# Frontend Mentor - Tech book club landing page solution

This is a solution to the [Tech book club landing page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/tech-book-club-landing-page-fZQidjHU73). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the interface depending on their device's screen size
- See hover and focus states for all interactive elements on the page

### Links

- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned


```less
span {
    position: relative;
    z-index: 1;
}
span::before {
    content: "";
    position: absolute;
    background: url(./assets/images/pattern-circle.png) no-repeat;
    background-size: 100% 100%;
    width: 6.75rem;
    height: 2.875rem;
    left: -15%;
}
```
* Positioned orange circle with full size, using ::before to place it behind the text, and flipped its intrinsic width & height to size it on the screen. 
* Took inspiration from:  https://mzdemir-tech-book-club-landing-page.netlify.app/.

```less
  .container3 {
      position: relative;
      padding-inline: 1.5rem;
      .text {
          .header {
              .tp2();
              span::before {
                  width: 9.875rem;
                  height: 4.25rem;
                  left: -15%;
              }
          }
      }
      .tech-logos {
          position: absolute;
          z-index: 1;
          display: block;
          left: 70%;
          top: 80%;
      }
  }
```
* Calculated the % of the positions using the Figma orange lines and the size of the container in Figma to get the percentages for positioning the tech-logos.

### Continued development

Going to start using React.js and CSS Modules to shorten time spent on working on projects.
Keep testing myself of positioning images and background patterns etc.

## Author

- Frontend Mentor - [@lemz100](https://www.frontendmentor.io/profile/lemz100)

## Acknowledgments

Credit to https://mzdemir-tech-book-club-landing-page.netlify.app/. for the club orange circle positioning.
