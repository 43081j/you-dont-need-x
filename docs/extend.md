# extend

You can use object spread to achieve shallow cloning (i.e. extend/merge
functionality):

```ts
const merged = {
  ...sourceObject,
  ...sourceObject2,
  key: val
};
```

Almost always, you do not need a library to do this.

In modern browsers, you also have the `structuredClone` API available for
deep clones of objects:

https://web.dev/structured-clone/
