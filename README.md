# umi-plugin-sentry

[![NPM version](https://img.shields.io/npm/v/umi-plugin-sentry.svg?style=flat)](https://npmjs.org/package/umi-plugin-sentry)

Umi plugin for sentry.

## Install

```bash
yarn add --dev umi-plugin-sentry # OR npm install --save-dev umi-plugin-sentry
```

## Use

Just setup the plugin on `.umirc.js`

```js
export default {
  plugins: [
    // ...
    ['umi-plugin-sentry', options],
    // ...
  ],
}
```

## Options

| name                               | type                             | default                                      |
|------------------------------------|----------------------------------|----------------------------------------------|
| dsn                                | string (required in production)  | `process.env.SENTRY_DSN`                     |
| log (log to console before send)   | boolean (optional)               | `NODE_ENV === 'development' ? true : false`  |
| environment                        | string (optional)                | ``                                           |
