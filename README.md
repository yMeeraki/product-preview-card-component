# Frontend Mentor - Product preview card component solution

This is a solution to the [Product preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
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

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

### Links

- Solution URL: [Github](https://github.com/yMeeraki/product-preview-card-component)
- Live Site URL: [Netlify](https://previewproduct-fem.netlify.app)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

Throughout this project, I deepened my knowledge in responsive web design, semantic HTML, and Flexbox for layout management. Here are some specific areas I focused on:

1. **Responsive Images with `<picture>` Element**: 
   I used the `<picture>` element to serve different image sources depending on the user's screen size, ensuring that the appropriate image is loaded for mobile and desktop views. This not only improves loading speed but also enhances the overall user experience.

   ```html
   <picture>
     <source media="(min-width: 1024px)" srcset="./images/image-product-desktop.jpg">
     <img src="./images/image-product-mobile.jpg" alt="Product Image">
   </picture>
   ```

2. **CSS Flexbox for Layouts**:
Flexbox was used to create a responsive card layout. By adjusting the flex-direction based on the screen size, I ensured that the card content adapts to both mobile and desktop displays.

    ```css
    .card {
      display: flex;
      flex-direction: column;
      max-width: 20rem;
    }

    @media (min-width: 768px) {
      .card {
        flex-direction: row;
        max-width: 40rem;
      }
    }
    ```

3. **Button Hover Effects**:
I also added hover effects to enhance the user experience. The button changes color when hovered over, making it more interactive.

```css
.add-button:hover {
  background-color: hsl(212, 21%, 14%);
}
```

### Continued development

Moving forward, I plan to focus on the following areas for continued development:

1. **CSS Grid Layouts**:  
   While I used Flexbox for this project, I aim to become more comfortable with CSS Grid for creating more complex, grid-based layouts. I want to explore how it complements Flexbox in responsive design.

2. **Advanced Responsive Design**:  
   I plan to dive deeper into media queries and learn more about using modern CSS features like `clamp()`, `minmax()`, and `aspect-ratio` to create fluid, adaptable layouts without hard breakpoints.

3. **JavaScript Interactivity**:  
   Although this project was mostly HTML and CSS, I want to incorporate more JavaScript in future projects to add dynamic features, such as form validation and interactive animations.

4. **Performance Optimization**:  
   Understanding how to optimize images, CSS, and scripts for faster load times, especially on mobile devices, is something I’ll continue working on. Techniques like lazy loading and code splitting are areas I'd like to explore further.

By focusing on these areas, I aim to create more complex, efficient, and user-friendly projects in the future.


### Useful resources

- [MDN Web Docs - Responsive Images](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images) - This article helped me understand how to properly use the `<picture>` element and `srcset` attribute for responsive images. It's a comprehensive guide that I'd recommend to anyone looking to improve their responsive image handling.
- [CSS Tricks - A Complete Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) - This guide was essential in helping me get a firm grasp on Flexbox for creating responsive layouts. I constantly referred back to it throughout the project and will continue to use it in the future.
- [Google Fonts](https://fonts.google.com/) - This resource was useful for selecting the right typography for my project. I found it easy to integrate custom fonts using Google Fonts.


## Author

- Linkedin - [Yukti Gupta](https://www.linkedin.com/in/yukti-gupta-589974195/)
- Frontend Mentor - [@yMeeraki](https://www.frontendmentor.io/profile/yMeeraki)

