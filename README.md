# json function loader for webpack

## Installation

`npm install --save json-function-loader`

## Usage
Wraps json in a function. This allows a pristine object to be returned on each function call. Helpful in testing to prevent mutation affecting unrelated tests.

``` javascript
var json = require("json-function!./file.json")();
// => returns file.json content as json parsed object
```

Don't forget to polyfill `require` if you want to use it in node.
See `webpack` documentation.

## License

MIT (http://www.opensource.org/licenses/mit-license.php)
