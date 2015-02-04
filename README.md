# Polyfill for `Object.setPrototypeOf`

A simple cross platform implementation to set the prototype of an instianted object.  Supports all modern browsers and at least back to IE8.

## Usage:

```javascript
var setPrototypeOf = require('setprototypeof');

var obj = {};
setPrototypeOf(obj, {
	foo: function() {
		return 'bar';
	}
});
obj.foo(); // bar
```
