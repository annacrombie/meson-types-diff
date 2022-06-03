# meson-types-diff

This repo contains type signatures for meson functions.  The type signatures
come from 3 sources, with each source getting its own branch.

- refman\_types - These types come from the official meson docs (`docs/yaml` in
  the meson repo).
- typed\_types - These types come from meson's `@typed_kwargs` and
  `@typed_posargs` function decorators.
- annotated\_types - These types come from the python type annotations of the
  functions.  In cases where there are no annotations, types from the above
  function decorators are used as fallbacks.  Additionally posargs annotations
  are not used since I haven't found a way to differentiate between posargs and
  varargs.

Note: for both typed\_types and annotated\_types, the return type of the
function comes from the python annotation since there is no decorator that
provides return type information.

- [refman\_types..typed\_types](https://github.com/annacrombie/meson-types-diff/compare/refman_types..typed_types)
- [refman\_types..annotated\_types](https://github.com/annacrombie/meson-types-diff/compare/refman_types..annotated_types)
- [typed\_types..annotated\_types](https://github.com/annacrombie/meson-types-diff/compare/typed_types..annotated_types)
