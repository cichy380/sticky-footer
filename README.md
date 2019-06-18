# Sticky footer
Pin a flexible-height footer to the bottom of the viewport in desktop browsers with this custom HTML and CSS.

CSS:
```css
html {
    height: 100%;
}
body {
    height: 100%;
    display: flex;
    flex-direction: column;
}
main {
    flex: 1 1 auto;
}
```
Note:
definition `flex-grow: 1` causes `<main/>` fill the all available space

HTML:

```html
<header>header</header>
<main>content</main>
<footer>footer</footer>
```
Live preview: https://jsfiddle.net/cichy380/sm9pdyhw/
