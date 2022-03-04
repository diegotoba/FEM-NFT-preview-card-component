# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Links

- Solution URL: [https://github.com/diegotoba/FEM-NFT-preview-card-component](https://github.com/diegotoba/FEM-NFT-preview-card-component)
- Live Site URL: [https://brave-keller-57dc39.netlify.app/](https://brave-keller-57dc39.netlify.app/)

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox

### What I learned

I got to learn a way to make an image hover overlay, wich I managed to do like this:

.nft-image-active{
  position: absolute;
  top: 0;
  left: 0;
  height: 100%;
  width: 100%;
  border-radius: 20px;
  background-color: #00fff77a;
  opacity: 0;
}

.nft-image-active-icon {
  position: absolute;
  top: 45%;
  left: 42%;
}

.nft-image-active:hover {
  opacity: 1;
}

Later, advice from the FrontEndMentor community gave me a better looking solution, making the hover effect CSS only:

.nft-picture::after {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  height: 100%;
  width: 100%;
  border-radius: 20px;

}

.nft-picture:hover::after, .nft-picture:active::after {
  background: #00fff77a url(./images/icon-view.svg) center/3rem no-repeat;
}
### Useful resources

https://www.w3schools.com/howto/howto_css_image_overlay.asp

## Author

- Frontend Mentor - [@diegotoba](https://www.frontendmentor.io/profile/diegotoba)
