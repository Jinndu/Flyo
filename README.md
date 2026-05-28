[README.md](https://github.com/user-attachments/files/28353223/README.md)
# Frontend Mentor - Fylo data storage component solution

This is a solution to the [Fylo data storage component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/fylo-data-storage-component-1dZPRbV5n). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
  - [AI Collaboration](#ai-collaboration)
- [Author](#author)
- [Acknowledgments](#acknowledgments)


## Overview
This project is a responsive Fylo data storage component built with only HTML and CSS.  

The goal of the project was to recreate the provided Frontend Mentor design while practicing layout structuring, positioning, responsive design, gradients, and custom UI components.
The interface contains:
- A logo and icon section
- A storage information card
- A custom progress slider
- A floating storage notification
- Responsive desktop and mobile layouts


### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size

### Screenshot


### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process
### HTML Structure

The project structure was divided into two main containers:

 Left Container
Contains:
- Fylo logo
- Document, folder, and upload icons

 Right Container
Contains:
- Storage usage text
- Custom slider/progress bar
- Storage range labels
- Floating storage information box

Semantic nesting and reusable class naming were used to keep the layout organized.


 ### Layout and Positioning

Flexbox was used throughout the project for alignment and spacing.

Main techniques used:
- `display: flex`
- `justify-content`
- `align-items`
- `flex-direction`
- `gap`

The body layout changes from:
- Column layout on mobile
- Row layout on desktop

using media queries.

 Background Styling

Different background images were used for:
- Mobile view
- Desktop view

The background image behavior was controlled using:

```css
background-position
background-size: cover
background-repeat: no-repeat
``` 
 ### Custom Slider Creation
The storage progress bar was recreated using pure CSS.

The slider consists of:

A dark outer track
A gradient-filled progress section
A white circular indicator

Techniques used:

linear-gradient()
border-radius
position: relative
::after pseudo-element

The white circle was attached using a pseudo-element positioned at the edge of the gradient fill.

### Floating Storage Box

The "185 GB LEFT" card was positioned using absolute positioning.

On desktop:

  - A triangular tail was added using borders
  - The effect was created with a pseudo-element

  ```css
  border-top: 20px solid white;
  border-left: 20px solid transparent;
  ```

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Media-query


### What I learned
I learnt how to properly utilize the flexbox better. 
I had some issues on divs floating around outside their parent div when the screen size was reduced or increased 
Solution: 
I used min-height and min-width to rectify this. Also I stopped the habit of using percentage for important parent divs(vh, px or rem is preferrable)

Also in building a realistic slider, i attempted to use ::-webkit-slider-thumb, ::-webkit-slider-runnable-track


### Continued development

I'm hoping to learn more on 
 - box-shadow
 - responsive mobile and web dev
 - min-height and min-width
 - flexbox 
 - pseudo elements


### Useful resources

- https://developer.mozilla.org/en-US/docs/Web/CSS/Reference



## Author

- Website - [Jinndu](https://github.com/Jinndu)
- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/Jinndu)
- Twitter - [@yourusername](https://x.com/agu_bliss)

