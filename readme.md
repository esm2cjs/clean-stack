# @esm2cjs/clean-stack

This is a fork of https://github.com/sindresorhus/clean-stack, but automatically patched to support ESM **and** CommonJS, unlike the original repository.

## Install

You can use an npm alias to install this package under the original name:

```
npm i clean-stack@npm:@esm2cjs/clean-stack
```

```jsonc
// package.json
"dependencies": {
    "clean-stack": "npm:@esm2cjs/clean-stack"
}
```

but `npm` might dedupe this incorrectly when other packages depend on the replaced package. If you can, prefer using the scoped package directly:

```
npm i @esm2cjs/clean-stack
```

```jsonc
// package.json
"dependencies": {
    "@esm2cjs/clean-stack": "^ver.si.on"
}
```

## Usage

```js
// Using ESM import syntax
import cleanStack from "@esm2cjs/clean-stack";

// Using CommonJS require()
const cleanStack = require("@esm2cjs/clean-stack").default;
```

> **Note:**
> Because the original module uses `export default`, you need to append `.default` to the `require()` call.

For more details, please see the original [repository](https://github.com/sindresorhus/clean-stack).

## Sponsoring

To support my efforts in maintaining the ESM/CommonJS hybrid, please sponsor [here](https://github.com/sponsors/AlCalzone).

To support the original author of the module, please sponsor [here](https://github.com/sindresorhus/clean-stack).
