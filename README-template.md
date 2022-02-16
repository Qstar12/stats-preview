# Frontend Mentor - Stats preview card component solution

This is a solution to the [Stats preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/stats-preview-card-component-8JqbgoU62). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size

### Screenshot

![](/images/statespreview.png.png)
![](/images/statspreviewdesktop.png.png)



### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow
- [Styled Components](https://styled-components.com/) - For styles

### What I learned

Which this challenge I chose to give grid a go. I learned that it was the best way to go in order to have full control of separte card components and to place them where I needed them. I also learned a bit about the accent color that overlays the image. The way that I figured this out was to use '''mix-blend-mode: darken;''' on the child element. 

```scss
.hero {
    width: 327px;
    height: 240px;
    object-fit: cover;
    border-radius: 8px 8px 0 0; 
    overflow: hidden; 
    background-repeat: no-repeat;
    background-size: cover;
    border: none;
    position: relative;
    margin-bottom: 2.5em;
    background-color: hsla(277, 64%, 61%, 0.7);
    
    
    &::before {
        content: '';
        background-image: url(/images/image-header-mobile.jpg);
        position: absolute;
        top: 0;
        bottom: 0;
        left: 0;
        right: 0;
        background-size: cover;
        mix-blend-mode: multiply;
        
        @media (min-width: 77.5em) {
            background-image: none;   
        } 

    } 

}
```

If you want more help with writing markdown, we'd recommend checking out [The Markdown Guide](https://www.markdownguide.org/) to learn more.


### Continued development

In future project I believe that I will continue to work with grid. I still need to get the concept down as well as identify other use case where grid is more beneficial than flex.


## Author

- Website - [Amario Jones](https://www.your-site.com)
- Frontend Mentor - [@Qstar12](https://www.frontendmentor.io/profile/Qstar12)
- Twitter - [@jones_amario](https://twitter.com/jones_amario)



## Acknowledgments

Thanks for viewing! 
