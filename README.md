# Utility CSS

Simple and easy to use utilities CSS, inspired by [tailwindcss](https://github.com/tailwindcss/tailwindcss), but the tailwindcss is more complex and verbose to use. This only focused on wrap the most common use css into class name. The most utilities steal from [Bootstrap](https://github.com/twbs/bootstrap) utilities.

Not support Responsive.

## Usage

```
npm install utilities-css
```

Or from CDN

```
<link href="https://unpkg.com/utilities-css" rel="stylesheet">
```

## Utilities

#### Display

The naming is `disply-{value}`, {value} is one of `none, inline, inline-block, block, table, table-row, table-cell, flex, inline-flex, grid`.

#### Float

Be ware the float utilities have no affect on flex items. `float-{value}`, {value} is one of `left, right, none`

#### Position

The naming is `position-{value}`, {value} is one of `static, relative, absolute, fixed, sticky`.

#### Visibility

The naming is `visible` or `invisible`

#### Overflow

The naming as blow

- `overflow-{value}`, {value} is one of `visible, hidden, scroll, auto`
- `overflow-{x|y}-{value}`, {value} is one of `visible, hidden, scroll, auto`

#### z-index

The naming is `z-{value}`, {value} for 0|10|20|30|40|50|auto

#### Colors

text colors:

`.text-{value}`, {value} for `primary, secondary, light, dark, muted, white`. if applied with `<a>` or `<button>` element, which have a hover state for darken 10%.

background colors:

`.bg-{value}`, {value} for `primary, secondary, light, dark, white , transparent`. also when background color applied with `<a>` or `<button>` elements, which have a hover state for darken 10%;

#### Spacing

The classes are named using the format `{property}{sides}-{size}`

The {property} is one of:

- m - for classes that set margin
- p - for classes that set padding

Where {sides} is one of:

- t - for classes that set margin-top or padding-top
- b - for classes that set margin-bottom or padding-bottom
- l - for classes that set margin-left or padding-left
- r - for classes that set margin-right or padding-right
- x - for classes that set both _-left and _-right
- y - for classes that set both _-top and _-bottom
- blank - for classes that set a margin or padding on all 4 sides of the element

Where {size} is one of:

- 0 - for classes that eliminate the margin or padding by setting it to 0
- 1 - for classes that set the margin or padding to \$spacer \* .25
- 2 - for classes that set the margin or padding to \$spacer \* .5
- 3 - for classes that set the margin or padding to \$spacer
- 4 - for classes that set the margin or padding to \$spacer \* 1.5
- 5 - for classes that set the margin or padding to \$spacer \* 3
- auto - for classes that set the margin to auto

> the `$spacer` default 1rem

Example:  
`mt-0` set the element margin-top with 0 value  
`px-0` set the element padding left and right with 0 value  
`mx-auto` set the element margin left and right with auto value

#### Shadow

The shadow utility copied from bootstrap.

- `shadow-none`
- `shadow-sm`
- `shadow`
- `shadow-lg`

#### Border

The border default width is `1px solid #6c757d`

- `border`
- `border-top`
- `border-right`
- `border-bottom`
- `border-left`

Border style:

- `border-solid`
- `border-dashed`
- `border-dotted`
- `border-none`

Border width:

- `.border-{0|1|2|3|4|5}`
- `.border-{top|right|bottom|left}-{0|1|2|3|4|5}`

Border color:  
`border-{color}`, the color is one of `primary, secondary, light, dark, muted, white`.

Border radius:

- `rounded`
- `rounded-{sm|lg}` radius size
- `rounded-{top|right|bottom|left}`
- `rounded-{top|right|bottom|left}-{sm|lg}`
- `rounded-circle` circle
- `rounded-0` no radius

#### Sizing

- `w-{25|50|75|100|auto}` for width 25%, 50%, 75%, 100% and auto
- `h-{25|50|75|100|auto}` for height 25%, 50%, 75%, 100% and auto
- `mw-100` set the max-width with 100%
- `mh-100` set the max-height with 100%

#### Flex

Support most features of flex layout and let user quickly manage layout, alignment and more of control. steal from Bootstrap flex utilities.

- flex direction
    - flex-row
    - flex-row-reverse
    - flex-column
    - flex-column-reverse
- flex wrap
    - flex-wrap
    - flex-nowrap
    - flex-wrap-reverse
- flex grow and shrink
    - flex-fill
    - flex-grow-0
    - flex-grow-1
    - flex-shrink-0
    - flex-shrink-1
- justify content
    - justify-content-start
    - justify-content-end
    - justify-content-center
    - justify-content-between
    - justify-content-around
- align items
    - align-items-start
    - align-items-end
    - align-items-center
    - align-items-baseline
    - align-items-stretch
- align content
    - align-content-start
    - align-content-end
    - align-content-center
    - align-content-between
    - align-content-around
    - align-content-stretch
- align self
    - align-self-auto
    - align-self-start
    - align-self-end
    - align-self-center
    - align-self-baseline
    - align-self-stretch
    
#### Others

Other utilities

- clearfix

## publish

- run `npm version major|minor|patch -m "some message %s"`
- run `npm publish`

## Contributing

If you're interested in contributing to Utilities CSS, please read our [CONTRIBUTING.md](https://github.com/buuug7/utilities-css/blob/master/CONTRIBUTING.md) before submitting a pull request.
