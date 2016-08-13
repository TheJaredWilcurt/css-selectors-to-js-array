# css-selectors-to-js-array

This is a javascript library that can be ran in the browser or with Node.js.

This library converts any valid CSS string passed in to an array of all its selectors.

[Live Demo on Codepen](http://codepen.io/TheJaredWilcurt/full/grQQqV/)


* * *


## USE

```html
 <script type="text/javascript" src="selectorstoarray.min.js"></script>
```

```js
// Variable containing any valid CSS as a string
var css = 'h1 { font-size: 10px; } .thing h4 .moo:nth-child(-2n+3) a[href*="#"] i:after { content: ""; border: 0px; width: 0px } h2 {}';

// Pass in any valid CSS into the selectorsToArray function
var selectors = selectorsToArray(css);

// Return an array of CSS Selectors in the order they were in the CSS file with none removed/missing
console.log(selectors); // [ 'h1', '.thing h4 .moo:nth-child(-2n+3) a[href*="#"] i:after', 'h2' ];
```


* * *

## CONTRIBUTE

* We definately need to do a lot more vigorous testing to make sure this library works with any valid CSS file. FILE BUGS!
* We should probably get this registered on NPM so others can use the library and keep up to date with bug fixes.
* [This guy had some good ideas](https://www.reddit.com/r/learnjavascript/comments/4wsxg4/how_do_i_create_a_js_array_of_css_selectors_from/d6bs2wk?context=10000)


* * *


## USED BY

Currently this library is used by the repo it was created for:

* [ITCSS: Specificity Graph](https://github.com/TheJaredWilcurt/itcss-specificity-graph)
 
If you use this library in a project, let us know by filing an issue to have your link added, or doing a pull request edit of the README.


* * *


## LICENSE

Public domain homie, do with as you will.
