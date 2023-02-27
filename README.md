# Frontend Mentor - Product preview card component solution

This is a solution to the [Product preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

### Screenshot

![](./Screenshot-desktop-view.png)

Add a screenshot of your solution. The easiest way to do this is to use Firefox to view your project, right-click the page and select "Take a Screenshot". You can choose either a full-height screenshot or a cropped one based on how long the page is. If it's very long, it might be best to crop it.

Alternatively, you can use a tool like [FireShot](https://getfireshot.com/) to take the screenshot. FireShot has a free option, so you don't need to purchase it. 

### Links

- Solution URL: [Solution Repo](https://github.com/shashikantdev3/FrontendMentor-Challange-product-preview-card-component-main)
- Live Site URL: [Live Preview](https://shashikantdev3.github.io/FrontendMentor-Challange-product-preview-card-component-main/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow
- [Styled Components](https://styled-components.com/) - For styles


### What I learned

While creating the Product preview card I tried to use best practices for HTML and CSS. In this project I have learned how to make a website suitabke for screenreader and Visually hidden techniques which allow for content to be hidden from sighted users while still allowing ATs to discover and interact with the content.

learned about :is() selector in CSS

Also, learned more details about responsiveness and breakpoints.

See below code for screen only text and a great way to add SVG and TEXT to a button. 

```html
   <div class="flex-group">
          <p class="product__discount-price">
            <span class="sr-only">Discount Price</span>
            $149.99
          </p>
          <p class="product__original-price">
            <span class="sr-only">Original Price</span>
            <s>$169.99</s>
          </p>
        </div>
        
  <button class="button" data-icon="shopping-cart">Add to Cart</button>
```
```css
.sr-only:not(:focus):not(:active) {
    clip: rect(0 0 0 0); 
    clip-path: inset(50%);
    height: 1px;
    overflow: hidden;
    position: absolute;
    white-space: nowrap; 
    width: 1px;
  }
}

  .button[data-icon="shopping-cart"]::before{
    content: "";
    background-image: url(./images/icon-cart.svg);
    width: 15px;
    height: 16px;
  }
```
### Useful resources

- [Example resource 1](https://www.joshwcomeau.com/css/custom-css-reset/) - This helped me to reset the CSS. I really liked this pattern and will use it going forward.
- [Example resource 2](https://www.scottohara.me/blog/2017/04/14/inclusively-hidden.html) - This is an amazing article which helped me Visually hidden techniques to make the website more accessible to screen reader and visually impaired person. I'd recommend it to anyone still learning this concept.


## Author

- Website - [Shashikant](https://www.your-site.com)
- Frontend Mentor - [@shashikantdev3](https://www.frontendmentor.io/profile/shashikantdev3)
- Twitter - [@shashikantdev3](https://www.twitter.com/shashikantdev3)

