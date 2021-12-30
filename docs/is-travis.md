# is-travis

To detect if you're running in Travis or not, you do not and should not need
a dependency.

```ts
const isInTravis = 'TRAVIS' in process.env;
```

As specified in Travis' own
[docs](https://docs.travis-ci.com/user/environment-variables/#default-environment-variables).
