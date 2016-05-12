# LESS Long Shadow

This [LESS](http://lesscss.org/) loop mixins generates trendy flat long shadow with any angle for inline text, font icons, block elements and SVGs. Looks best if wrapped by square `overflow: hidden;` container with _bold_ padding and rounded corners. Dont forget about good contrast color palette. Enjoy!

* Source: [GitHub](https://github.com/zensimilia/less-long-shadow)
* Demo: [CodePen](http://codepen.io/zensimilia/full/XbVgNx/)
* Author: [Di M Dub](https://twitter.com/zensimilia)

## Installation

1. Make shure that you [installed](http://lesscss.org/) client or server-side LESS css-preprocessor
2. [Clone git repo](https://github.com/zensimilia/less-long-shadow/fork) or [Download](https://github.com/zensimilia/less-long-shadow/archive/master.zip) and copy `long-shadow.less` to your _e.g._ `/assets/less` directory
3. Plug it to project by insert `@import "long-shadow.less";` at beginning of main LESS/CSS stylesheet file
4. Assign mixins to elements rules.
5. PROFIT

## Usage

```less
.someClass {
    #long-shadow.inline(@color, @angle, @size); // For text or icon
    #long-shadow.block(@color, @angle, @size, @prefix); // For container
    #long-shadow.svg(@color, @angle, @size, @prefix); // For SVG
}
```

## Params

* __@color__ of shadow _e.g._ `#00FFFF`, `@someVariable` or [`darken(#00FFFF)`](http://lesscss.org/functions/#color-operations-darken):
  * Default `#CCCCCC`.
* __@angle__ of shadow from 0 to 360. Zero meant horizontal shadow with right direction:
  * Default `45`.
* __@size__ that shadow length would be:
  * Default `10`.
* __@prefix__ param define the use of CSS _browser-prefixes_ for `box-shadow` or `filter` rule:
  * `0` : _false_
  * `1` : _true_ Default

> Be careful with large values of the param `size` with client-side compiling. Using LESS in the browser is great for development, but it's not recommended for production due low performance.

## Contributing & Issues

Have a bug or a feature request? [Please open a new issue](https://github.com/zensimilia/less-long-shadow/issues). Before opening any issue, please search for existing issues.

## TODO

- [ ] Correctly implement spread transparency.
- [x] Add support for shadows on SVG.
- [x] Add ability to specify an angle of shadow.

## Changelog

__2.1.0__
* Add support for shadows on SVG by [Randall Bruder](https://github.com/randybruder).

__2.0.0__
* __INCOMPATIBLE CHANGES!__ Add _namespace_ and rename mixins.
* Add ability to specify an _angle_ of shadow. Idea [Mark Campbell](https://github.com/artsmc).
* Add option to choose whether to use _browser-prefixes_.
* Remove _spread_ parameter. Now total flat shadow.

__1.0.0__
* Initial release.

## License

[MIT License](LICENSE.md)
