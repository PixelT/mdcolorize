Simple sass (SCSS) function for fast usage [material design colors](https://material.io/resources/color)

## Installation:
npm: `npm install mdcolorize`<br>
yarn: `yarn add mdcolorize`

then:

`@import 'mdcolorize';`

## Usage:

`mdcolorize($palette, $value, $alpha);`
<br><br>
**palette** (required) - one of 19 defined color palettes:
<br>
`$color_amber`
`$color_blue`
`$color_blueGrey`
`$color_brown`
`$color_cyan`
`$color_deepOrange`
`$color_deepPurple`
`$color_green`
`$color_grey`
`$color_indogo`
`$color_lightBlue`
`$color_lightGreen`
`$color_lime`
`$color_orange`
`$color_pink`
`$color_purple`
`$color_red`
`$color_teal`
`$color_yellow`
<br><br>
Additionally:
`$color_black`
`$color_white`
<br><br>
**value** (optional) - value of the color. Default `500`
<br>
`50` `100` `200` `300` `400` `500` `600` `700` `800` `900`<br>
*optionally, for some palettes:*
`a100`
`a200`
`a400`
`a700`
<br><br>
**alpha** (optional) - opacity of the color, value must be between `0` and `1`

## Examples:

```
color: mdcolorize($color_red); // #f44336
color: mdcolorize($color_red, 100); // #ffcdd2
color: mdcolorize($color_red, 700, .5); // rgba(211, 47, 47, 0.5)
```
```
color: mdcolorize($color_white); // #fff
color: mdcolorize($color_white, $alpha: .1); // rgba(255, 255, 255, 0.1)
color: mdcolorize($color_black); // #000
color: mdcolorize($color_black, $alpha: .1); // rgba(0, 0, 0, 0.1)