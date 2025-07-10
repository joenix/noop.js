# noop.js

## 1. Install

```sh
npm i noop.js
# or
yarn add noop.js
# or
pnpm i noop.js
```

## 2. Import

```js
import noop from 'noop.js';
// or
import { noop } from 'noop.js';
```

## 3. Use

```js
noop(); // Nothing

const fn = (callback = noop) {
    callback();
}
```

## 4. Promise

```js
import { noopPromise } from 'noop.js';

const fn = async (callback = noopPromise) => {
  await callback();
};
```
