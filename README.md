# LESS Long Shadow

This [LESS](http://lesscss.org/) loop mixins generates flat-trendy long shadows for any inline-text, font-icons or block-elements. Looks best if wrapped by square `overflow: hidden;` block with _bold_ padding and 25% rounded corners. Dont forget about good contrast color palette!

* Source: [https://github.com/zensimilia/less-long-shadow](https://github.com/zensimilia/less-long-shadow)
* Author Twitter: [@zensimilia](https://twitter.com/zensimilia)

## Installation

1. Make shure that you [installed](http://lesscss.org/) client- or server-side LESS css-preprocessor
2. [Clone git repo](https://github.com/zensimilia/less-long-shadow/fork) or [Download](https://github.com/zensimilia/less-long-shadow/archive/master.zip) and copy `long-shadow.less` to your _e.g._ `/assets` directory
3. Plug it to project by insert `@import "long-shadow.less";` at beginning of main LESS/CSS stylesheet file
4. Assign mixins to elements. Enjoy!

## Usage

```css
.box {
	overflow: hidden;

	.longShadow(@color, @size, @spread);
	.longShadowBox(@color, @size, @spread);
}
```

## Params

* __@color__ of shadow _e.g._ `#00FFFF`, `@buttonShadowColor` or `darken(#00FFFF)`.
* __@size__ in pixels that shadow would be.
* __@spread__ shadow opacity. Greater value - straighter edges. Defaults:
 * longShadow: __100__
 * longShadowBox: __1__

## Issues

Have a bug or a feature request? [Please open a new issue](https://github.com/zensimilia/less-long-shadow/issues). Before opening any issue, please search for existing issues.

## Changelog

__1.0__
* Initial release

## Copyright and license

[MIT License](LICENSE.md)