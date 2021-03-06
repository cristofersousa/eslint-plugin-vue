# enforce attribute naming style in template (attribute-hyphenation)

- :wrench: The `--fix` option on the [command line](http://eslint.org/docs/user-guide/command-line-interface#fix) can automatically fix some of the problems reported by this rule.

## :wrench: Options

Default casing is set to `always`

```
'vue/attribute-hyphenation': [2, 'always'|'never']
```

### `"always"` - Use hyphenated name. (It errors on upper case letters.)

:+1: Examples of **correct** code`:

```html
<template>
  <foo my-prop="prop">
    <a onClick="return false"></a>
  </foo>
</template>
```

:-1: Examples of **incorrect** code`:

```html
<template>
  <foo myProp="prop">
    <a onClick="return false"></a>
  </foo>
</template>
```

### `"never"` - Don't use hyphenated name. (It errors on hyphens except `data-` and `aria-`.)

:+1: Examples of **correct** code`:

```html
<template>
  <foo myProp="prop">
    <a onClick="return false"></a>
  </foo>
</template>
```

:-1: Examples of **incorrect** code`:

```html
<template>
  <foo my-prop="prop">
    <a onClick="return false"></a>
  </foo>
</template>
```
