# Fozzie Colour Palette

[![npm version](https://badge.fury.io/js/%40justeat%2Ffozzie-colour-palette.svg)](https://badge.fury.io/js/%40justeat%2Ffozzie-colour-palette)
[![Build Status](https://travis-ci.org/justeat/fozzie-colour-palette.svg)](https://travis-ci.org/justeat/fozzie-colour-palette)

This module allows projects to import the Just Eat brand colour palette, so that they can always stay up to date with any changes made.

Colours are made available by a number of Sass variables that once the module has been imported can be referenced in a projects Sass files.

[Zeplin colour palette](https://zpl.io/ZTch33)

## Usage

1. The easiest way to use fozzie modules in your Sass setup is to use [Eyeglass](https://www.npmjs.com/package/eyeglass).

If you are using the [fozzie gulp build tasks](https://www.npmjs.com/package/@justeat/gulp-build-fozzie), then Eyeglass is automatically setup ready to use.  If not, you can use it in one of the following ways:

- [Gulp](https://github.com/sass-eyeglass/eyeglass/blob/master/site-src/docs/integrations/gulp.md)
- [WebPack](https://github.com/sass-eyeglass/eyeglass/issues/153#issuecomment-300895607)

2.  Install the fozzie-colour-palette module using NPM or Yarn:

    ```bash
    yarn add @justeat/fozzie-colour-palette
    ```

3.  Then within your Sass files, you will need to import this module.

    ```scss
    @import 'fozzie-colour-palette';
    ```

You can then use any of the colour variables [contained in the module](https://github.com/justeat/fozzie-colour-palette/blob/master/src/scss/index.scss).

It’s recommended that you hook onto and use the variable abstractions such as `$color-text` and `$color-link-default` where it makes sense to, rather than directly onto the colour variables.  That way your project will require less re-factoring should the colour palette ever get a major overhaul in the future and certain colours get replaced and/or renamed.


## Available Colour Schemes

The `fozzie-colour-palette` allows for the definition of platform specific colour schemes.  The colour schemes currently available are:

### Just Eat Default Colour Scheme

To apply the default Just Eat colour scheme, simply import this module like so:

```scss
  @import 'fozzie-colour-palette';
```

If you are already importing the [base `fozzie` module](https://www.npmjs.com/package/@justeat/fozzie) there will be no need to import `fozzie-colour-palette` as this is baked in by default to that module.  The default colour scheme will therefore automatically be setup when importing the base `fozzie` module.


###  Menulog Colour Scheme

To apply the Menulog colour palette, you need to import the default colour scheme, and then call the `applyScheme-menulog` mixin, which provides a set of theme overrides.

To do this, define a `$theme` variable  and set it to `'ml'`.  Then conditionally call the Menulog colour scheme mixin:

```scss
  $theme: 'ml';

  @import 'fozzie-colour-palette';

  @if ($theme == 'ml') {
      @include applyScheme-menulog;
  }
```

If you are using the base `fozzie` module, simply setting the `$theme: 'ml';` before importing the `fozzie` module will automatically take care of this step for you:

```scss
  $theme: 'ml';

  @import 'fozzie'; // this will now load in the fozzie-colour-palette module with Menulog overrides
```

