# Frontend Mentor - Order summary card solution

This is a solution to the [Order summary card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/order-summary-component-QlPmajDUj).

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)

## Overview

### The challenge

Users should be able to:

- Build out this order summary card component and get it looking as close to the design as possible.
- See hover states for interactive elements

### Screenshot

![desktop-design](https://user-images.githubusercontent.com/58538880/138966012-aa6e5fe5-eadc-49f6-8c9a-60e1401945dd.jpg)

![mobile-design](https://user-images.githubusercontent.com/58538880/138966017-a7b37da6-4ea8-43bc-af69-465b1377dc4d.jpg)

### Links

- Live Site URL: [Live Demo](https://rluna15.github.io/order-summary-component/)

## My process

### Built with

- HTML5
- Sass
- Gulp (Sass Compiler)


### What I learned

```html
<button class="btn btn-blue">Process Payment</button>
```

```css
@use "../util/" as u;
@use "../globals/" as g;

.btn {
    margin-top: 30px;
    padding: 15px;
    width: 100%;
    border-radius: 10px;
    border: none;

    &-blue {
        background-color: g.$Bright-blue;
        font-weight: bold;
        color: g.$White;
        font-family: g.$Red-Hat;

        &:hover{
            background-color: lighten(g.$Bright-blue, 15%);
        }
    }

    &-link {
        color: g.$Desaturated-blue;
        background: none;
        font-weight: bold;
        font-family: g.$Red-Hat;

        &:hover{
            color:  darken(g.$Desaturated-blue, 20%);
        }
    }
    
}
```
