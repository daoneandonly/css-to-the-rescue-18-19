# Assignment

A random grid layout (based on the time of day) with random shapes done with SVG.

## (Possible) Restrictions

My idea has to have ~~at least~~ two restricions. I'm not sure which, but I'll choose one of the following.

- No squares, no rectangles, no circles, no triangles
- Responsive without media queries
- Two colours
- Less than 5kb CSS

## Idea

Using SVG Geographical shapes from the provinces of The Netherlands to form a layout.

### Content

My content will exist of a page that's about one of the provinces of the Netherlands, North-holland.

## Results, methods and problems

This whole subject was process of learning the restrictions of css. While working with svg, I figured out there's a lot you can do with them but mostly when they're inline.

- I've tried using the SVG `clipPath` to hide/mask certain content. However `clipPath` doesn't work with a `path` svg element.
  (Used reference: [One](https://codepen.io/abbeyjfitzgerald/pen/mELOpy), [two](https://codepen.io/abbeyjfitzgerald/pen/dXZXNr).)

- I figured out how to individually style paths in an inline svg. [Link to CodePen](https://codepen.io/Pantheratnight/pen/KJvrJY)

- Using `shape-outside` to align text to a svg. `shape-outside` requires you to have an image next to the text, using `float` and reference that same image in css through `shape-outside: url(image.svg)`.
  [Link to CodePen](https://codepen.io/Pantheratnight/pen/xMpbGx) This worked through CodePen, with a placeholder svg. However locally I keep getting errors with loading in the `shape-outside: url(image.svg)`.

- Found out that shape-inside is no longer supported.

- viewBox is a p.i.t.a to work with.

- I've applied a gradient on a svg using the `<defs>` element. Gradients work a little different than css `linear-gradient()`. They require a `<linearGradient>` element with `<stop>` elements nested inside of them. Learned this at **Fronted United** from [Lea Verou](https://www.frontendunited.org/speakers/lea-verou). 👍

- With the element `<animate>` inside of an svg, I animated the before mentioned lineaerGradient `<stop>` to change the gradient. 🎉🎉

- More gradients!!! 🔴🔵🔴 Found a way to give text a gradient. It's a bit of a hack, but with a `-webkit-background-clip:text;` and `-webkit-text-fill-color:transparent;`, you can gradient the background and "fill" the text with that color. [Source.](https://css-tricks.com/snippets/css/gradient-text/)

- Using `filter:hue-rotate()` on a image gives some awesome trippy effects!
