# Frontend Mentor - Order summary card solution

This is a solution to the [Order summary card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/order-summary-component-QlPmajDUj). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Frontend Mentor - Order summary card solution](#frontend-mentor---order-summary-card-solution)
  - [Table of contents](#table-of-contents)
  - [Overview](#overview)
    - [The challenge](#the-challenge)
    - [Screenshot](#screenshot)
    - [Links](#links)
  - [My process](#my-process)
    - [Built with](#built-with)
    - [What I learned](#what-i-learned)
    - [Continued development](#continued-development)
  - [Author](#author)

## Overview

### The challenge

Users should be able to:

- See hover states for interactive elements

### Screenshot

![](screenshot.png)

### Links

- Solution URL: [Frontend Mentor](https://www.frontendmentor.io/challenges/order-summary-component-QlPmajDUj/hub/order-summary-component-css-flexbox-CUbgRVwqcd)
- Live Site URL: [Vercel](https://order-summary-component-arjjkq0yg-justinnvera.vercel.app)

### Built with

- Semantic HTML5 markup
- CSS utility class
- Flexbox

### What I learned

I learned how to use the `overflow: hidden` trick on my `.container` tag while having the border-radius in it. This is useful since it also 'applies' the border-radius to all its child elements since `overflow: hidden` hides overlapping child elements. The code is shown below:

```html
<div class="container">
    <img class="hero-image" src="/images/illustration-hero.svg" alt="" aria-hidden="true">
    <div class="order-summary">
        <h1>Order Summary</h1>
        <p>You can now listen to millions of songs, audiobooks, and podcasts on any device anywhere you like!</p>    
    </div>
    <div class="annual-plan">
        <img src="/images/icon-music.svg" alt="" aria-hidden="true">
        <div class="annual-plan-text">
            <h4 class="plan-type">Annual Plan</h4>
            <span class="price">$59.99/year</span>
        </div>
        <a class="change-plan hover-state" href="#">Change</a>
    </div>
    <div class="checkout">
        <button class="proceed hover-state" type="submit">Proceed to Payment</button>
        <a class="cancel hover-state" href="#">Cancel Order</a>
    </div>
</div>
```
```css
.container {
    border-radius: 20px;
    overflow: hidden;
}
```
I also learned how to create a CSS utility class to save lines of code which I decided to implement on the elements that had hover states. Below are some examples:

```html
<div class="container">
    <img class="hero-image" src="/images/illustration-hero.svg" alt="" aria-hidden="true">
    <div class="order-summary">
        <h1>Order Summary</h1>
        <p>You can now listen to millions of songs, audiobooks, and podcasts on any device anywhere you like!</p>    
    </div>
    <div class="annual-plan">
        <img src="/images/icon-music.svg" alt="" aria-hidden="true">
        <div class="annual-plan-text">
            <h4 class="plan-type">Annual Plan</h4>
            <span class="price">$59.99/year</span>
        </div>
        <a class="change-plan hover-state" href="#">Change</a>
    </div>
    <div class="checkout">
        <button class="proceed hover-state" type="submit">Proceed to Payment</button>
        <a class="cancel hover-state" href="#">Cancel Order</a>
    </div>
</div>
```
```css
.hover-state:hover {
    cursor: pointer;
    opacity: 0.8;
}
```

### Continued development

I feel that I've got that CSS positioning down and I'd like to expland my knowledge and experience by taking on multi-layout projects. However, if there is anything I can improve upon, feel free to let me know. I'm always happy to receive a message :)

## Author

- Website - [Justin Vera](https://www.justinvera.com)
- Frontend Mentor - [@justinnvera](https://www.frontendmentor.io/profile/justinnvera)
