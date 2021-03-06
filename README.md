LoMein - Signal Style Guide
===========================

LoMein is a base style sheet for Signal's brand.  [See Demo Here](http://signal.github.io/lo-mein/)

Usage
-----

LoMein is designed to be included as a ready-to-use CSS style sheet or as a SASS library that allows you to use stylistic variables in your own SASS files.

### Include CSS Style Sheet

LoMein can be installed by simply adding the [latest CSS file](https://github.com/BrightTag/LoMein/releases/latest/) to the `<head>` of your web page:

```html
<link rel="stylesheet" type="text/css" href="lo-mein.css">
```

### Use as a SASS Library

ake sure you have [npm](https://www.npmjs.com/), [gulp](http://gulpjs.com/), [ruby](https://www.ruby-lang.org/) and [bundler](http://bundler.io/) installed on your machine.  Next install the library using npm:

```bash
npm install --save git://github.com/signal/lo-mein.git
```

Include LoMein at the top of your SCSS file:

```scss
@import 'node_modules/lo-mein/styles/_config.scss';
```

Now all of the lo-mein styles will be available as variables in your SCSS file. These variables are defined in the [styles/config](styles/config) directory and includes several different files which can be used as a reference:

- [_colors.scss](styles/config/_colors.scss): The colors used with Signal's brand. (e.g. `$signal-red`)
- [_dimensions.scss](styles/config/_dimensions.scss): Dimensions of text and elements. (e.g. `$lo-border-radius`)
- [_font-stacks.scss](styles/config/_font-stacks.scss): Font families used in signal materials. (e.g. `$proxima-nova`)
- [_layout.scss](styles/config/_layout.scss): Includes grid layout variables (`$grid`) and responsive breakpoints (`$breakpoints`).

Development
-----------

Make sure you have [npm](https://www.npmjs.com/), [gulp](http://gulpjs.com/), [ruby](https://www.ruby-lang.org/) and [bundler](http://bundler.io/) installed on your machine.

**To install:** `npm install`

**To build resources:** `gulp`

**To watch:** `gulp watch`

**To serve documentation:** `gulp serve`

**To deploy the documentation:** `gulp deploy` Note that this will only work for Signal employees.

