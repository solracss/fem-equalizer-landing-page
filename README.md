# Frontend Mentor - [Equalizer landing page ](https://www.frontendmentor.io/challenges/equalizer-landing-page-7VJ4gp3DE).

## Deployed site
[![live](https://github.com/solracss/fem-equalizer-landing-page/assets/19937659/8f3ca94f-9136-4725-b53f-a13b215dde0a)](https://solracss.github.io/fem-equalizer-landing-page/)

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [How to run](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### How to run

1. Clone repo
2. Open cli

```
npm install
npm run dev
```

## My process

### Built with

[![My Skills](https://skillicons.dev/icons?i=html,css,sass,vscode,vite)](https://skillicons.dev)

### What I learned

1. Keep footer always on bootom of page

```css
body {
	display: flex;
	flex-direction: column;
}

footer {
	margin-top: auto;
}
```

other way with grid, worth to add some margin-top for footer

```css
body {
	display: grid;
	grid-template-rows: auto 1fr auto; // depends how many parts page have
}
```

2. Work with positioning elements. Whole middle section required to position phone image and cta box differently depending on what screen size user displays page.

3. Use `clamp` for dynamic width for heading

```css
.top-section-wrapper {
	width: clamp(32rem, 65vw, 53rem);
}
```

4. Work with `grid` to display footer elements.

5. Use styles for button links as predefined component class.
