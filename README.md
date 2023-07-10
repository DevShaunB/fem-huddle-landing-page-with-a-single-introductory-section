# Frontend Mentor - Huddle landing page with single introductory section solution

This is a solution to the [Huddle landing page with single introductory section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/huddle-landing-page-with-a-single-introductory-section-B_2Wvxgi0). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [Reference](#reference)
  - [Color](#color)
  - [Typography](#typography)
- [Run Locally](#run-locally)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the page depending on their device's screen size
- See hover states for all interactive elements on the page

### Screenshot

![Huddle landing page with single introductory section desktop screenshot](https://devshaunb.github.io/fem-huddle-landing-page-with-a-single-introductory-section/screenshots/desktop.png)

![Huddle landing page with single introductory section mobile screenshot](https://devshaunb.github.io/fem-huddle-landing-page-with-a-single-introductory-section/screenshots/mobile.png)

### Links

- Live Site URL: [https://devshaunb.github.io/fem-huddle-landing-page-with-a-single-introductory-section/](https://devshaunb.github.io/fem-huddle-landing-page-with-a-single-introductory-section/)

## Reference

### Color

#### Primary

- ![hsl(257, 40%, 49%)](https://via.placeholder.com/10/674baf?text=+) `Violet: hsl(257, 40%, 49%)`
- ![hsl(300, 69%, 71%)](https://via.placeholder.com/10/e882e8?text=+) `Soft Magenta: hsl(300, 69%, 71%)`

#### Neutral

- ![hsl(0, 0%, 100%)](https://via.placeholder.com/10/ffffff?text=+) `White: hsl(0, 0%, 100%)`
- ![hsl(0, 0%, 0%)](https://via.placeholder.com/10/000000?text=+) `Black: hsl(0, 0%, 0%)`

### Typography

#### Headings

- Family: [Poppins](https://fonts.google.com/specimen/Poppins)
- Weights: 400, 600

#### Body

- Family: [Open Sans](https://fonts.google.com/specimen/Open+Sans)
- Weights: 400

## Run Locally

Clone the project

```bash
  git clone https://github.com/DevShaunB/fem-huddle-landing-page-with-a-single-introductory-section.git
```

Go to the project directory

```bash
  cd fem-huddle-landing-page-with-a-single-introductory-section/
```

Run `index.html`

```bash
  <browsername> index.html
```

E.g.

```bash
  firefox index.html
```

```bash
  google-chrome index.html
```

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

- creating accessible list of social icons

```html
<ul class="footer__social-list">
  <li class="footer__social-item">
    <a href="/" class="footer__social-link"
      ><span class="sr-only">Huddle on Facebook</span
      ><i class="fa-brands fa-facebook-f" aria-hidden="true"></i
    ></a>
  </li>
  <!-- and so on -->
</ul>
```

- using `container` to keep content from stretching too far on bigger screens

```html
<main class="main">
  <div class="container">
    <div class="main__img-wrapper">
      <img src="./images/illustration-mockups.svg" alt="" class="main__img" />
    </div>
    <div class="main__content">
      <h1 class="main__title">Build...</h1>
      <p class="main__desc">Huddle...</p>
      <a href="/" class="main__cta">Register</a>
    </div>
  </div>
</main>
```

- creating anchor tag link that look like button

```css
a {
  display: inline-block;
  text-decoration: none;
  color: inherit;
}

.main__cta {
  font-size: 0.75rem;
  padding: 1em 6.25em 0.75em;
  background-color: hsl(var(--clr-white));
  color: hsl(var(--clr-violet-400));
  border-radius: 5em;
  box-shadow: 0 0.5em 0.67em hsl(var(--clr-black) / 0.25);
  outline: transparent;
}
```

- creating circle outlined links

```css
.footer__social-link {
  width: 2em;
  height: 2em;
  border: 1px solid;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  border-radius: 50%;
  outline: transparent;
}
```

- responsive font with `clamp`

```css
.main__title {
  font-size: clamp(1.5rem, 2.78vw, 2.5rem);
}
```

## Author

- Frontend Mentor - [@DevShaunB](https://www.frontendmentor.io/profile/DevShaunB)
- Twitter - [@DevShaunB](https://www.twitter.com/DevShaunB)

## Acknowledgments

- [Huddle landing page with single introductory section challenge](https://www.frontendmentor.io/challenges/huddle-landing-page-with-a-single-introductory-section-B_2Wvxgi0) by [Frontend Mentor](https://www.frontendmentor.io/)
- [Font Awesome](https://fontawesome.com/)
