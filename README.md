# YACCK
YACCK - Yet Another Classless CSS Kit  

[Live demo](https://spncrhrstn.github.io/yacck/)  

YACCK is a classless, responsive CSS kit/framework that focuses on pure HTML elements. It is inspired by many other similar minimal CSS frameworks, such as [MVP.css](https://github.com/andybrewer/mvp) and [new.css](https://github.com/xz/new.css). Meant for use in simple websites and blogs.

Currently a work in progress.

## Goals
* Simple universal layout
* Cross-browser support
* Responsive
* Accessible (as much as possible)
* Customization

## HTML Layout
YACCK follows a somewhat opinionated way of laying your HTML. See the [demo page](https://spncrhrstn.github.io/yacck/) for an example layout.

## Customizing
YACCK uses CSS variables in the `:root` element to define customizable values, such as sizing, colors and fonts.  

You can override the defaults in your own CSS file in a `:root` rule. 

### Fonts
By default, YACCK uses a font stack of system fonts for sans-serif and monospace, so no external fonts required. However, you are welcome to use your own fonts. The following fonts (in my opinion) work well:

Sans-Serif
* [**Rubik**](https://fonts.google.com/specimen/Rubik)
* [Inter](https://fonts.google.com/specimen/Inter)
* [DM Sans](https://fonts.google.com/specimen/DM+Sans)
* [Roboto](https://fonts.google.com/specimen/Roboto)
* [Nunito](https://fonts.google.com/specimen/Nunito)
* [Heebo](https://fonts.google.com/specimen/Heebo)

Monospace
* [**Fira Mono**](https://fonts.google.com/specimen/Fira+Mono)
* [Inconsolata](https://fonts.google.com/specimen/Inconsolata)
* [DM Mono](https://fonts.google.com/specimen/DM+Mono)
* [Roboto Mono](https://fonts.google.com/specimen/Roboto+Mono)
* [Cousine](https://fonts.google.com/specimen/Cousine)

Add a link to the fonts in your HTML's `<head>`:

```html
<link href="https://fonts.googleapis.com/css2?family=Fira+Mono&family=Rubik&display=swap" rel="stylesheet">
```

In your own CSS file, add a reference to the fonts in the `:root` element:

```css
:root{
    --font-family: 'Rubik', Roboto, 'Segoe UI', Helvetica, Arial, sans-serif;
    --font-monospace: 'Fira Mono', 'Roboto Mono', Consolas, 'Courier New', Courier, monospace;
}
```

*Note that Rubik and Fira Mono are already referenced by default in `yacck.css`. You just need to be sure to link to the fonts in your HTML files.*

## Acknowledgements
Example page based on [HTML5 Test Page](https://github.com/cbracco/html5-test-page). Inspired by [MVP.css](https://github.com/andybrewer/mvp), [new.css](https://github.com/xz/new.css) and other minimal CSS frameworks (see list [here](https://github.com/dohliam/dropin-minimal-css)).
