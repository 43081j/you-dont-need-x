# import-from

Modules like this exist to `require()` from directories other than the default
one of the current file.

The node API supports this directly:

```ts
const {createRequire} = require('module');
const path = require('path');

const requireCwd = createRequire(path.resolve(process.cwd(), '_'));
requireCwd('./some-file');
```

Using the same pattern, you can require from any given path:

```ts
const {createRequire} = require('module');

const requireFromPath = createRequire(somePath);
requireFromPath('./some-file');
```
