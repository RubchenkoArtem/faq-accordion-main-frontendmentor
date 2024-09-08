# Frontend Mentor - FAQ accordion solution

This is a solution to the [FAQ accordion challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/faq-accordion-wyfFdeBwBz). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Solutions](#solutions)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### The challenge

![](./design/desktop-preview.jpg)

Your challenge is to build out this FAQ accordion and get it looking as close to the design as possible.

You can use any tools you like to help you complete the challenge. So if you've got something you'd like to practice, feel free to give it a go.

Your users should be able to:

Hide/Show the answer to a question when the question is clicked
Navigate the questions and hide/show answers using keyboard navigation alone
View the optimal layout for the interface depending on their device's screen size
See hover and focus states for all interactive elements on the page

### Solutions

- Solution URL: [Click]()
- Live Site URL: [Click]()

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Media query
- CSS Web Fonts
- JavaScript

### What I learned

```js
accordionBtns.forEach(btn => {
    btn.addEventListener('click', function() {
        this.classList.toggle('active')
        const accordionDescription = this.nextElementSibling
        const plusIcon = this.querySelector('.plus-icon')
        const minusIcon = this.querySelector('.minus-icon')

        if(accordionDescription.style.maxHeight) {
            accordionDescription.style.maxHeight = null
            plusIcon.style.display = 'block'
            minusIcon.style.display = 'none'
        } else {
            accordionDescription.style.maxHeight = accordionDescription.scrollHeight + 'px'
            plusIcon.style.display = 'none'
            minusIcon.style.display = 'block'   
        } 
    })
```
### Useful resources

- [W3school](https://www.w3schools.com/css/css3_fonts.asp) - This is an amazing website which helped me finally understand CSS Web Fonts. I'd recommend it to anyone still learning this concept.

## Author

- Website - [Artem Rubchenko](https://github.com/RubchenkoArtem)
- Frontend Mentor - [@RubchenkoArtem](https://www.frontendmentor.io/profile/RubchenkoArtem)
- Twitter - [@94Blackwalker](https://x.com/94Blackwalker)