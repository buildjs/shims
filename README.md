# shimmer

This is a [bakeable](https://github.com/DamonOehlman/bake-js) collection of shims for Javascript Objects that might not be implemented in older browsers.  The majority of the functions have been implemented directly from the excellent [es5-shim](https://github.com/kriskowal/es5-shim) repository.

The reason this repository exists is to facilitate only pulling in shims that are required by your library, rather than including all ES5 functionality.

## Usage

If you are building a Bake ready Javascript library, then simply add a `req` comment for the particular shims you require, e.g.

```js
// req: shimmer[js#Array.forEach, js#Array.filter]

[1,2,3].forEach(function(value) {
    
});
```
