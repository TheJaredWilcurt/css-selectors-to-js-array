# css-selectors-to-js-array

This is a javascript library that can be ran in the browser or with Node.js.

This library converts any valid CSS string passed in to an array of all its selectors.

[Live Demo on Codepen](http://codepen.io/TheJaredWilcurt/full/grQQqV/)

## USE

```
var css = 'h1 { font-size: 10px; } .thing h4 .moo:nth-child(-2n+3) a[href*="#"] i:after { content: ""; border: 0px; width: 0px } h2 {}';
var selectors = selectorsToArray(css);
console.log(selectors); // [ 'h1', '.thing h4 .moo:nth-child(-2n+3) a[href*="#"] i:after', 'h2' ];
```
