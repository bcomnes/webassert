# `webassert`

> Nanoscale assertion esm module

A fork of [nanoassert](https://ghub.io/nanoassert) porting it over to real-deal ESM.  Directly importable to browsers (also works in node).

## Usage

```js
import assert from 'https://unpkg.com/webassert@^3?module'

assert(a !== b, `${a} !== ${b}`)
```

## API

### `assert(declaration, [message])`

Assert that `declaration` is truthy otherwise throw `AssertionError` with
optional `message`. In Javascript runtimes that use v8, you will get a nicer
stack trace with this error.
If you want friendlier messages you can use template strings to show the
assertion made like in the example above.

## Why

> I like to write public facing code very defensively, but have reservations about
the size incurred by the `assert` module. I only use the top-level `assert`
method anyway.

I liked nanoassert but wanted an ESM version of it.

## Install

```sh
npm install nanoassert
```

## License

[ISC](LICENSE)
