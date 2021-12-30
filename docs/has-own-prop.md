# has-own-prop

To determine if an object has a property or not safely, you can simply use:

```ts
Object.prototype.hasOwnProperty.call(obj, prop);
```

In future, you may be able to use `Object.hasOwn(obj, prop)` as
explained here:

https://github.com/tc39/proposal-accessible-object-hasownproperty
