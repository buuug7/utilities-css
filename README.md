# Utility CSS

Simple and easy to use utilities CSS, inspired by [tailwindcss](https://github.com/tailwindcss/tailwindcss), but the
tailwindcss is more complex and verbose to use. This only focused on wrap the most common used css into class name. Most
of them is steal from [Bootstrap](https://github.com/twbs/bootstrap) utilities.

 <p>
    <a href="https://www.npmjs.com/package/utilities-css?minimal=true">
        <img src="https://img.shields.io/npm/v/utilities-css.svg" alt="npm version">
  	</a>
  	<a href="https://npmcharts.com/compare/utilities-css?minimal=true">
  	    <img src="https://img.shields.io/npm/dm/utilities-css.svg" alt="npm downloads"> 
  	</a>
  	<a href="#">
  	   <img src="https://img.shields.io/bundlephobia/min/utilities-css.svg" alt="minified size"/>
  	</a>
 </p>

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

The naming is `display-{value}`, `{value}` is one
of `none, inline, inline-block, block, table, table-row, table-cell, flex, inline-flex, grid`.

```html
<div class="display-block">some text</div>
```

#### Float

Beware the float utilities have no effect on flex items. `float-{value}`, `{value}` is one of `left, right, none`.

```html
<div class="float-left">some text</div>
```

#### Position

The naming is `position-{value}`, `{value}` is one of `static, relative, absolute, fixed, sticky`.

```html
<div class="position-relative">some text</div>
```

#### Visibility

The naming is `visible` or `invisible`.

```html
<div class="invisible">some text</div>
```

#### Overflow

The naming as blow

- `overflow-{value}`, {value} is one of `visible, hidden, scroll, auto`
- `overflow-{x|y}-{value}`, {value} is one of `visible, hidden, scroll, auto`

```html
<div class="overflow-hidden">some text</div>
<div class="overflow-x-hidden">some text</div>
```

#### z-index

The naming is `z-{value}`, {value} for 0|10|20|30|40|50|auto

```html
<div class="z-10">some text</div>
```

#### Spacing

The classes are naming using the format `{property}{sides}-{size}`

The `{property}` is one of:

- **m** for classes that set margin
- **p** for classes that set padding

Where {sides} is one of:

- **t** for classes that set margin-top or padding-top
- **b** for classes that set margin-bottom or padding-bottom
- **l** for classes that set margin-left or padding-left
- **r** for classes that set margin-right or padding-right
- **x** for classes that set both _-left and _-right
- **y** for classes that set both _-top and _-bottom
- **blank** for classes that set a margin or padding on all 4 sides of the element

Where {size} is one of:

- **0** for classes that eliminate the margin or padding by setting it to 0
- **1** for classes that set the margin or padding to `$spacer * .25`
- **2** for classes that set the margin or padding to `$spacer * .5`
- **3** for classes that set the margin or padding to `$spacer`
- **4** for classes that set the margin or padding to `$spacer * 1.5`
- **5** for classes that set the margin or padding to `$spacer * 3`
- **auto** for classes that set the margin to auto

> the `$spacer` default 1rem

Example:

```html
<!-- mt-0 set the element margin-top with 0 value -->
<div class="mt-0">some text</div>

<!-- px-0 set the element padding left and right with 0 value -->
<div class="px-0">some text</div>

<!-- mx-auto set the element margin left and right with auto value -->
<div class="mx-auto">some text</div>
```

#### Shadow

The shadow utility copied from bootstrap.

- `shadow-none`
- `shadow-sm`
- `shadow`
- `shadow-lg`

```html
<div class="shadow-sm">some text</div>
```

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

Border radius:

- `rounded`
- `rounded-{sm|lg}` radius size
- `rounded-{top|right|bottom|left}`
- `rounded-{top|right|bottom|left}-{sm|lg}`
- `rounded-circle` circle
- `rounded-0` no radius

```html
<div class="border-top border-dashed rounded-top">some text</div>
```

#### Sizing

- `w-{25|50|75|100|auto}` for width 25%, 50%, 75%, 100% and auto
- `h-{25|50|75|100|auto}` for height 25%, 50%, 75%, 100% and auto
- `mw-100` set the max-width 100%
- `mh-100` set the max-height 100%
- `w-100` set width 100%
- `h-100` set height 100%
- `wh-100` set both the with and height 100%

```html
<div class="w-100">some text</div>
```

#### Flex

Support most features of flex layout and let user quickly manage the layout, alignment and more of control. steal from
Bootstrap flex utilities.

- flex direction
  - `flex-row`
  - `flex-row-reverse`
  - `flex-column`
  - `flex-column-reverse`
- flex wrap
  - `flex-wrap`
  - `flex-nowrap`
  - `flex-wrap-reverse`
- flex grow and shrink
  - `flex-fill`
  - `flex-grow-0`
  - `flex-grow-1`
  - `flex-shrink-0`
  - `flex-shrink-1`
- justify content
  - `justify-content-start`
  - `justify-content-end`
  - `justify-content-center`
  - `justify-content-between`
  - `justify-content-around`
- align items
  - `align-items-start`
  - `align-items-end`
  - `align-items-center`
  - `align-items-baseline`
  - `align-items-stretch`
- align content
  - `align-content-start`
  - `align-content-end`
  - `align-content-center`
  - `align-content-between`
  - `align-content-around`
  - `align-content-stretch`
- align self
  - `align-self-auto`
  - `align-self-start`
  - `align-self-end`
  - `align-self-center`
  - `align-self-baseline`
  - `align-self-stretch`
- other
  - flex-center (display flex and set both horizontal and vertical center)

```html
<div class="display-flex justify-content-center align-content-center">
  some text
</div>
```

#### font

font weight

- `fw-light` font weight with 300
- `fw-normal` font weight with 400
- `fw-bold` font weight with 700

font style

- `fst-italic` font-style with italic
- `fst-normal` font-style with normal

font size

- `fs-1` font-size with 2.5rem , it related to h1
- `fs-2` font-size with 2rem , it related to h2
- `fs-3` font-size with 1.75rem , it related to h3
- `fs-4` font-size with 1.5rem , it related to h4
- `fs-5` font-size with 1.25rem , it related to h5
- `fs-6` font-size with 1rem , it related to h6

#### text

text align

- `text-align-start` text-align with left
- `text-align-end` text-align with right
- `text-align-center` text-align with center

white space

- `text-wrap` white space with normal
- `text-nowrap` white space with nowrap

word break

- `text-break` with break-word

text transform

- `text-lowercase` text-transform with lowercase
- `text-uppercase` text-transform with uppercase
- `text-capitalize` text-transform with capitalize

text decoration

- `text-decoration-none` text-decoration with none
- `text-decoration-underline` text-decoration with underline
- `text-decoration-line-through` text-decoration with line-through

line height

- `lh-1` line-height with 1
- `lh-sm` line-height with 1.25
- `lh-base` line-height with 1.5
- `lh-lg` line-height with 2

text reset

- `text-reset` reset text color with parent

#### Other utilities

- `clearfix`
- `text-center`
- `list-unstyled`

## Contributing

If you're interested in contributing to Utilities CSS, please read
our [CONTRIBUTING.md](https://github.com/buuug7/utilities-css/blob/master/CONTRIBUTING.md) before submitting a pull
request.
