# css-selectors-to-js-array

This is a javascript library that can be ran in the browser or with Node.js.

This library converts any valid CSS string passed in to an array of all its selectors.

[Live Demo on Codepen](http://codepen.io/TheJaredWilcurt/full/grQQqV/)


* * *


## USE

```
 <script type="text/javascript" src="selectorstoarray.min.js"></script>
```

```
// Variable containing any valid CSS as a string
var css = 'h1 { font-size: 10px; } .thing h4 .moo:nth-child(-2n+3) a[href*="#"] i:after { content: ""; border: 0px; width: 0px } h2 {}';

// Pass in any valid CSS into the selectorsToArray function
var selectors = selectorsToArray(css);

// Return an array of CSS Selectors in the order they were in the CSS file with none removed/missing
console.log(selectors); // [ 'h1', '.thing h4 .moo:nth-child(-2n+3) a[href*="#"] i:after', 'h2' ];
```


* * *


## LICENSE

Public domain homie, do with as you will.
