# is-string & friends

Most of these packages exist for rare edge cases, or worse, are NPM clutter
(one line packages). Unfortunately many have found their way into general
usage, for which they are often unnecessary.

Almost everyone can go without these packages and use existing built-ins:

```ts
// Check for a string
typeof val === 'string';

// Check for NaN
Number.isNaN(val);

// Check for a number
typeof val === 'number';

// Check for a regexp
val instanceof RegExp;

// Check for a regexp without instanceof (usually not necessary)
Object.prototype.toString.call(val) === '[object RegExp]';

// Check for a plain object
Object.prototype.toString.call(val) === '[object Object]' &&
  val !== null;

// Check for a function
typeof val === 'function';
```
