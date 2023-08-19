# Teamway redesign

A redesign of Teamway found on [dribbble](https://dribbble.com/pleinhaus).

## Overview

![overview](https://www.rcboe.org/cms/lib/GA01903614/Centricity/Domain/17272/overview-icon-25.jpg)

- [Overview](#overview)
- [Screenshot](#screenshots)
- [Process](#process)
- [Technologies](#technologies)
- [Methodologies](#methodologies)
- [Challenges faced](#challenges-faced)
- [Lessons learned](#lessons-learned)
- [Resources](#resources)
- [Acknowledgements](#acknowledgements)
- [Live site](#live-site)
- [Author](#author)

## Screenshots

### Desktop

Please excuse some of the logos with background colors. 🙏
![Desktop view](/design/desktop-screenshot.png)

### Tablet

![Tablet view](/design/tablet-screenshot.png)

## Process

![Web design process](https://www.sphinx-solution.com/blog/wp-content/uploads/2020/07/top-10-web-design-trends.jpg)

### 1. Structure

Add all the required html structure without any styling. Add elements following semantics.

### 2. Style

Style the elements using CSS.

1. Add base styles
2. Add styles to elements from top to bottom

### 3. Breakpoints

Add breakpoint using media queries for screen sizes.

### 4. Readme

Write README.md

## Technologies

- [Html (Hypertext Markup Language)](https://developer.mozilla.org/en-US/docs/Web/HTML)
- [CSS (Cascading Style Sheet)](https://developer.mozilla.org/en-US/docs/Web/CSS)

## Methodologies

- Responsive Web Design
- CSS Grid
- CSS Flexbox
- Desktop first workflow

## Challenges Faced

### Implementing the "Hiring? book a call" button

```html
<div class="hire-cta">
    <a href="#" class="hire-cta-btn">
        <h2>Hiring? Book a call</h2>
        <div class="hire-cta-icon">
            <!-- svg -->
        </div>
    </a>
</div>
```

#### How I was able to style it

```css
.hire-cta-wrap {
    display: flex;
    width: 70%;
    justify-content: space-between;
    padding: 0;
    position: relative;
}

.hire-cta {
    width: 70%;
}

.hire-cta-btn {
    display: flex;
    justify-content: space-between;
    align-items: center;
    border-radius: 4rem;
    padding: .5em;
    color: rgba(249, 248, 245, 1);
    background-color: rgba(29, 33,37, 1);
}
```

### The Members grid

#### How I was able to implement it

```css
.members {
    width: 60%;
    display: grid;
    grid-template-rows: 1fr 25px 25px 1fr;
    gap: 1em;
    grid-template-areas: 
    "mike adaptable latisha"
    "mike adaptable rest"
    "mike asger rest"
    "remote asger rest"
    ;
}
```

## Lessons learned

- It is better to first visualize a grid's rows and columns on paper or something else before starting to implement it.  
It brings clarity to how many rows or columns you need.
This was very useful in implementing [the members grid](#the-members-grid).

- It better to use dynamic units like `rem` in media queries than to use specific widths like `px`.

## Resources

- [MDN Web Docs](https://developer.mozilla.org/en-US/). MDN helped me to learn all the techniques I used. Very useful resource.

## Acknowledgements

I'd like to thank:

- [@pleinhaus](https://dribbble.com/pleinhaus) from [Dribbble](https://dribbble.com) for the great design.

- My family for support.

- The Lord Almighty for provision of these capacities.

## Live site

Check out the live site [here](https://hirwankevin.github.io/teamway-redesign/). Feedback is much appreciated at:

## Author

- [📧 Email][def]

[def]: mailto:hirwankevin@gmail.com

- [✖ Twitter](https://twitter.com/kevinHirwaN)

- [🔗 LinkedIn](https://www.linkedin.com/in/kevin-hirwa-nzitatira-623022281/)
