# Frontend Mentor - Product preview card component solution

This is a solution to the [Product preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa). Coded by me.

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

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

### Screenshot

![screenshot of site](screenshot.png)

### Links

- Live Site URL: [https://lucasepk.github.io/perfume_website/](https://lucasepk.github.io/perfume_website/)

## My process

### Built with
- HTML
- CSS
- Flexbox

### What I learned
I learnt to use classes and ids in html properly (i think)

```html
<p class="gray_txt" id="perfume_txt">P E R F U M E</p>
<p class="bold_txt">Gabrielle Essence Eau De Parfum</p>
<p class="gray_txt">A floral, solar and voluptuous interpretation composed by Olivier Polge, Perfumer-Creator for the House of CHANEL.</p>
<span class="bold_txt" id="big_price">$149.99</span>
<s class="gray_txt" id="small_price">$169.99</s><br>
```

Learnt **flexbox** so I'm proud of this bad boys
```css
body{

    margin: 0px;/*To make it work with vh*/
    
    /*Centers all the content in body*/
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;


    background-color: hsl(30, 38%, 92%);
}

.flex_container{
    /*sets container as flex to make items align in rows*/
    max-width: 600px;
    max-height: 450px;
    display: flex;

    background-color: hsl(0, 0%, 100%);

    border-radius: 10px;
}
```
I also learnt about **media queries for mobile**! Thank god, it was really frustrating me not figuring out a solution on how to make the site responsive.
```css
@media(max-width:800px){ /*this needs to be put after the other code because of how css works*/
  .flex_container{
      /*Changes flex direction to column so objects go down instead of sideways*/
      flex-direction: column;
      /*I set the height manually because it overflowed idk why*/
      height: 700px;
      max-height: max-content; /*tbh idk what this does*/
      margin: 20px; /*This makes it so the borders of the window don't touch the container*/
  }

  #item1{
      /*changes background image*/
      background-image: url('images/image-product-mobile.jpg');
      width: 100%; /*makes image take all the width space of container*/
      min-height: 220px;

      /*changes borders so that it matches the new order*/
      border-radius: 10px 10px 0px 0px;
  }
}
```

### Continued development

I still want to continue to expand my understanding of flexbox, because sometimes things overflow and I don't really know why lol. I should also deepen my knowledge of html, because i'm probably writing things that work but that aren't good.

### Useful resources
- [w3schools](https://www.w3schools.com/) - Always has TONS of info which is super useful and well explained
- [https://youtu.be/fYq5PXgSsbE](https://youtu.be/fYq5PXgSsbE) - Video that taught me flexbox really well
- [https://developer.mozilla.org/en-US/docs/Web/CSS/background-size](https://developer.mozilla.org/en-US/docs/Web/CSS/background-size) - helped me understand how background image size works
- [https://youtu.be/qXRYMdvq_Dc](https://youtu.be/qXRYMdvq_Dc) - Video that taught me how to make image border roundness match the containers
- [https://youtu.be/Mkza0N8NiK4](https://youtu.be/Mkza0N8NiK4) - Video that taught me that media queries exist

## Author

- Frontend Mentor - [@LucasEPK](https://www.frontendmentor.io/profile/LucasEPK)
