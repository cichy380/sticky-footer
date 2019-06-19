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
definition `flex-grow: 1` causes `<main/>` fills the all available space

HTML:

```html
<!doctype html>
<html><!-- 100% height -->
    <head>
        <!-- ... -->
    </head>
    <body><!-- flex container / 100% height -->
        <header>header</header><!-- flex item -->
        <main>content</main><!-- flex item / fills the all available space -->
        <footer>footer</footer><!-- flex item -->
    <body>
</html>
```
Live preview: https://jsfiddle.net/cichy380/sm9pdyhw/
