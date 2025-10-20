# recipe-page-challenge

This is a solution to the [Recipe page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/recipe-page-KiTsR8QQKm).

## Table of contents

- [Overview](#overview)
  - [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

This is a recipe page blog displaying an image of the recipe followed by a simple description, ingredients, step to follow and it culminates with a table describing all the nutritional details at the end.

## My process

I started out with the basic html structure first. I divided the content into various sections to provide semantic meaning and also to be able to style the page effeciently by targeting one section at a time. I set up css variables for property values that i was supposed to reuse through the code. Then after centering the white card layout and assigning it a max-width i proceeded with styling my elements.

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

I learnt about pseudo elements and pseudo classes. Styling the numbers in the ordered list separately was something new for me.
.instructions-list > ol li::marker {
color: var(--brown-text-color);
font-weight: bold;
}
Similarly styling the borders except for the last row and styling both the columns in the table with diff text colors and font weights was a challenge for me and i am happy i was able to do it.
.data-table tr:not(:nth-last-child(1)) td {
border-bottom: 1px solid var(--border-color);
}
.data-table td:first-child {
color: var(--primary-text-color);
}
.data-table td:last-child {
color: var(--brown-text-color);
font-weight: bold;
}
