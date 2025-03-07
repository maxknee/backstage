# @backstage/errors

## 0.2.1

### Patch Changes

- 1ed305728b: Bump `node-fetch` to version 2.6.7 and `cross-fetch` to version 3.1.5
- c77c5c7eb6: Added `backstage.role` to `package.json`
- Updated dependencies
  - @backstage/types@0.1.2

## 0.2.0

### Minor Changes

- e2eb92c109: Removed the deprecated exports `ErrorResponse` and `parseErrorResponse`.

  Removed the deprecated `constructor` and the deprecated `data` property of `ResponseError`.

## 0.1.5

### Patch Changes

- 4d09c60256: Deprecate `parseErrorResponse` in favour of `parseErrorResponseBody`. Deprecate `data` field inside `ErrorResponse` in favour of `body`.
  Rename the error name for unknown errors from `unknown` to `error`.

## 0.1.4

### Patch Changes

- a15d028517: More API fixes: mark things public, add docs, fix exports
- 10615525f3: Switch to use the json and observable types from `@backstage/types`
- 8c30ae8902: Add `stringifyError` that is useful for logging e.g. `Something went wrong, ${stringifyError(e)}`

## 0.1.3

### Patch Changes

- 7e97d0b8c1: Add public tags and documentation
- 6077d61e73: Two new helpers have been added that make it easier to migrate to considering thrown errors to be of the type `unknown` in TypeScript. The helpers are `assertError` and `isError`, and can be called to make sure that an unknown value conforms to the shape of an `ErrorLike` object. The `assertError` function is a type-guard that throws in the case of a mismatch, while `isError` returns false.

  A new error constructor has also been added, `ForwardedError`, which can be used to add context to a forwarded error. It requires both a message and a cause, and inherits the `name` property from the `cause`.

## 0.1.2

### Patch Changes

- d1da88a19: Properly export all used types.
- Updated dependencies
  - @backstage/config@0.1.9
