<p align="center">
  <img src="docs/quikgrid.svg">
</p>
<p style="text-align: center">Painlessly simple CSS grids</p>

## Table of Contents
* [Quick Start](#quick-start)

## Why choose Quikgrid?

We love using libraries like Bootstrap and Tailwind. However these libraries contain lots of code you will likely never use, 

## Quick Start
There are multiple ways that you can integrate Quikgrid into your pipeline.

### Embed directly in HTML
You can use our CDN to get the most recent version and keep up to date. Just pop this in your `<head>` above your stylesheets.
```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/quikgrid/css/quikgrid.min.css">
```

Alternatively, you can [download the latest version](https://github.com/MattheousDT/quikgrid/releases/latest) of `quikgrid.min.css` and place it above your styles in the `<head>`

### via NPM
Install the package via NPM

```bash
npm i --save quikgrid
```

or by using Yarn

```bash
yarn add quickgrid
```

Now you can add the quikgrid files the way you'd like. If you are using SASS, I'd personally recommend including quikgrid's SASS entrypoint in your SCSS file as then you can use our functions and mixins, as well as change variables like column sizes, breakpoints etc.

Just add this above your code in your SASS file

```scss
@import "~quikgrid/sass/index.scss";
```

Alternatively, you can also import directly at the top of your JS file if you are using something like Webpack and you do not require our SASS breakpoints.


```js
import "quikgrid/css/quikgrid.css" // ES6 Import (Recommended for Webpack)

require("quickgrid/css/quikgrid.css") // ES5 and below
```