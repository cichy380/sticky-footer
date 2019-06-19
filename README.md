# Sticky footer
Pin a flexible-height footer to the bottom of the viewport in desktop browsers with this custom HTML and CSS.

#### CSS
```css
html, body {
    height: 100%;
}
body {
    display: flex;
    flex-direction: column;
}
main {
    flex: 1 0 auto;
}
footer {
  flex-shrink: 0;
}
```
Note:
declaration `flex-grow: 1` causes the element `<main/>` we want to grow to fill the all available space

#### HTML
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
