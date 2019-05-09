# include-media-visible-classes

An [include-media plugin](https://github.com/eduardoboucas/include-media) to generate visibility utility classes for showing elements at different breakpoints.

Largely a fork of [include-media-hidden-classes](https://github.com/eduardoboucas/include-media-hidden-classes)

## Usage

Import the `_include-media-visible-classes.scss` Sass partial and then include the `@include im-visible-classes();` mixin to generate the classes.

### Example

```scss
@import "_include-media-visible-classes";

@include im-visible-classes();
```

## Configuration

| Variable                     | Description                                                                      | Default                                                                                                          |
| ---------------------------- | -------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| `$im-visible-class`          | The base name to use for the classes.                                            | `'visible'`                                                                                                      |
| `$im-visible-use-important`  | Whether to generated classes with `!important;`                                  | `false`                                                                                                          |
| `$im-visible-include-exact`  | Whether to generate visiblity classes for min-width <= => max-width breakpoints. | `true`                                                                                                           |
| `$im-visible-include-down`   | Whether to generate visiblity classes for max-width breakpoints.                 | `true`                                                                                                           |
| `$im-visible-include-up`     | Whether to generate visiblity classes for min-width breakpoints.                 | `true`                                                                                                           |
| `$im-visible-exact-selector` | The breakpoint suffix to use to exact breakpoint classes.                        | `''`                                                                                                             |
| `$im-visible-up-selector`    | The breakpoint suffix to use to min-width breakpoint classes.                    | `'-up'`                                                                                                          |
| `$im-visible-down-selector`  | The breakpoint suffix to use to max-width breakpoint classes.                    | `'-down'`                                                                                                        |
| `$im-display-modes`          | A Sass map of display modes to generate classes for.                             | `(inline: inline, inline-block: inline-block, block: block, table: table, flex: flex, inline-flex: inline-flex)` |
