# Frontend Mentor - Social links profile solution

This is a solution to the [Social links profile challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/social-links-profile-UG32l9m6dQ). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

- See hover and focus states for all interactive elements on the page

### Screenshot
1. Desktop Screen

![](/screenshots/desktop-screen.png)

2. Mobile Screen

![](/screenshots/mobile-screen.png)

### Links

- Solution URL: (https://github.com/cia2003/fm-profile-links)
- Live Site URL: (https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox

### What I learned

I learned how to use pseudo-class to effectively define the color's global variable. Usually, I just copy-and-paste the color's code like below:

```css
main .content #profileCard {
    background-color: hsl(0, 0%, 12%);
    /* Other Codes */
}
```
But then, it will waste your time because you need to search it all over the page to copy other color. So, how do I solve it? I use :root pseudo-class to declare the color's global variable and use custom properties.

```css
:root {
    --Green: hsl(75, 94%, 57%);
    --White: hsl(0, 0%, 100%);
    --Grey-700: hsl(0, 0%, 20%);
    --Grey-800: hsl(0, 0%, 12%);
    --Grey-900: hsl(0, 0%, 8%);
}
```
After that, I try to use the :focus pseudo-class. I think this pseudo-class is helpful for accessibility: for people with low vision. So, you need to make the visual contrast from the base one.

for example, I use :focus to mark whether or not the button is being clicked.

![](/screenshots/focus-state.png)

### Continued development

I think I want to try something new: I want to learn how to use CSS Grid on the next project. Usually, I use flexbox because it is easy to use (if you understand how to use it :D).

### Useful resources

- [:root](https://developer.mozilla.org/en-US/docs/Web/CSS/:root) - This helped me to understand how :root pseudo-class works.
- [Declare Custom Properties](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_cascading_variables/Using_CSS_custom_properties#declaring_custom_properties) - This helped me to understand how to declare custom properties.
- [:focus](https://developer.mozilla.org/en-US/docs/Web/CSS/:focus) - This helped me to understand how :focus pseudo-class works.

## Author

- Frontend Mentor - [@cia2003](https://www.frontendmentor.io/profile/cia2003)

## Acknowledgments

- [@Axsel519](https://www.frontendmentor.io/profile/Axsel519) - I've got some inspiration from his solution in Frontend Mentor. In his code, he declare the color's global variable using :root pseudo-class.