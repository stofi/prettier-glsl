# Repository replicating a bug in `prettier-plugin-glsl`

This repository is a minimal example of a bug in `prettier-plugin-glsl`. The plug-in fails to format a file containing an `#include` directive.

## Steps to reproduce

1. Clone this repository
2. Run `npm install`
3. Run `npm run test`

## Expected result

The `test.glsl` file should be formatted correctly, with extra whitespace removed.

## Actual result
Prettier fails with a lexer error:

```
[error] test.glsl: Error: LEXER ERROR: unexpected character: ->"<- at offset: 9, skipped 1 characters.:
```


