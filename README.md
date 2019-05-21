# Assignment
A random grid layout (based on the time of day) with random shapes done with SVG.

## (Possible) Restrictions
My idea has to have ~~at least~~ two restricions. I'm not sure which, but I'll choose one of the following.

* No squares, no rectangles, no circles, no triangles
* Responsive without media queries
* Two colours
* Less than 5kb CSS ~~(this is gonna be tricky)~~

## Idea
Using SVG Geographical shapes from the provinces of The netherlands to form a layout.

### Content

My content will exist of


## Methods, errors and problems
I've tried the following methods to achieve my ideas

* I've tried using the SVG `clipPath` to hide/mask certain content. However `clipPath` doesn't work with a `path` svg element.
(Used reference: [One](https://codepen.io/abbeyjfitzgerald/pen/mELOpy), [two](https://codepen.io/abbeyjfitzgerald/pen/dXZXNr).)

* [Link to CodePen](https://codepen.io/Pantheratnight/pen/KJvrJY)

* Using `shape-outside` to align text to a svg. `shape-outside` requires you to have an image next to the text, using `float` and reference that same image in css through `shape-outside: url(image.svg)`.
[Link to CodePen](https://codepen.io/Pantheratnight/pen/xMpbGx) This worked through CodePen, with a placeholder svg. However locally I keep getting errors with loading in the   `shape-outside: url(image.svg)`.
