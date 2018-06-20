# Utility CSS

Simple and easy to use utilities CSS, inspired by [tailwindcss](https://github.com/tailwindcss/tailwindcss), but the tailwindcss is more complex and verbose to use. This only focused on wrap the most common use css into class name. this also compatibility with bootstrap utilities.  

The grid breakpoints is as same as bootstrap grid breakpoints. 
+ xs 0
+ sm 576px
+ md 768px
+ lg 992px
+ xl 1200px

## Usage
```
npm install utilities-css
```
Or from CDN
```
<link href="https://unpkg.com/utilities-css" rel="stylesheet">
```

## Include utilities

> The below {breakpoint} is one of `sm`, `md`, `lg` and `xl`

##### Display
The display utility referenced from bootstrap display utility. 

###### Normal
`.d-{value}`, value for `none, inline, inline-block, block, table, table-row, table-cell, flex, inline-flex`.

###### Responsive
`.d-{breakpoint}-{value}`,  be aware that `xs` in not include. value for `none, inline, inline-block, block, table, table-row, table-cell, flex, inline-flex`.

Example:  
`.d-md-hidden` which set the display of element with hidden value on `md` or wider


#### Float
The float utility referenced from bootstrap float utility. Be ware the float utilities have no affect on flex items.  

###### Normal
`.float-{value}`, value for `left, right, none`
+ `.float-left`
+ `.float-right`
+ `.float-none`

###### Responsive
`.float-{breakpoint}-{value}`, value for `left, right, none`.

Example:  
`.float-lg-right` which float right on `lg` or wider


#### Position
###### Normal
`.position-{value}`, value for `static, relative, absolute, fixed, sticky`.
+ `.position-static`
+ `.position-relative`
+ `.position-absolute`
+ `.position-fixed`
+ `.position-sticky`

###### Responsive
`.position-{breakpoint}-{value}`, value for `static, relative, absolute, fixed, sticky`.

Example:  
`.position-md-static` which set the element position with static value on `md` or wider


#### Visibility
+ `.visible`
+ `.invisible`


#### Overflow

###### Normal
+ `.overflow-{value}`, value for `visible, hidden, scroll, auto`
+ `.overflow-{x|y}-{value}`, value for `visible, hidden, scroll, auto`

###### Responsive
+ `.overflow-{breakpoint}-{value}`, value for `visible, hidden, scroll, auto`
+ `.overflow-{breakpoint}-{x|y}-{value}`, value for `visible, hidden, scroll, auto`

Example:
`.overflow-sm-hidden` which set the element overflow with hidden value on `sm` or wider screen


#### z-index
`.z-{value}`, value for 0|10|20|30|40|50|auto  

Example:  
`.z-10` for set the element z-index with 10 

#### Colors
###### text colors
`.text-{color}`, color for `primary, secondary, success info warning danger light dark muted white`. if applied with `<a>` or `<button>` element, which have a hover state for darken 10%.  

###### background colors
`.bg-{color}`, color for `primary secondary success info warning danger light dark white transparent`. also when background color applied with `<a>` or `<button>` elements, which have a hover state for darken 10%;

###### gradient background colors
`.bg-gradient-{color}`, color for `primary secondary success info warning danger light dark white transparent`.


#### Spacing
Referenced from bootstrap,the classes are named using the format `{property}{sides}-{size}` for xs and `{property}{sides}-{breakpoint}-{size}` for sm, md, lg, and xl.  

The property is one of:  
+ m - for classes that set margin
+ p - for classes that set padding

Where sides is one of:  
+ t - for classes that set margin-top or padding-top
+ b - for classes that set margin-bottom or padding-bottom
+ l - for classes that set margin-left or padding-left
+ r - for classes that set margin-right or padding-right
+ x - for classes that set both *-left and *-right
+ y - for classes that set both *-top and *-bottom
+ blank - for classes that set a margin or padding on all 4 sides of the element

Where size is one of:  
+ 0 - for classes that eliminate the margin or padding by setting it to 0
+ 1 - (by default) for classes that set the margin or padding to $spacer * .25
+ 2 - (by default) for classes that set the margin or padding to $spacer * .5
+ 3 - (by default) for classes that set the margin or padding to $spacer
+ 4 - (by default) for classes that set the margin or padding to $spacer * 1.5
+ 5 - (by default) for classes that set the margin or padding to $spacer * 3
+ auto - for classes that set the margin to auto

Example:  
`.mt-0` set the element margin-top with 0 value  
`.px-0` set the element padding left and right with 0 value  
`.px-sm-0` set the element padding left and right with 0 value on `sm` and wider  
`.mx-auto` set the element margin left and right with auto value

#### Shadow
This copied from bootstrap.
+ `.shadow-none`
+ `.shadow-sm`
+ `.shadow`
+ `.shadow-lg`

#### Border
The border default width is `1px solid #6c757d`
+ `.border`
+ `.border-top`
+ `.border-right`
+ `.border-bottom`
+ `.border-left`

Border style:  
+ `.border-solid`
+ `.border-dashed`
+ `.border-dotted`
+ `.border-none`

Border width: 
+ `.border-{0|1|2|3|4|5}`
+ `.border-{top|right|bottom|left}-{0|1|2|3|4|5}`

Border color:  
`.border-{color}`, the color is one of `primary, secondary, success, info, warning, danger, light, dark, muted, white`.

Border radius:  
+ `.rounded`
+ `.rounded-{sm|lg}` radius size
+ `.rounded-{top|right|bottom|left}`
+ `.rounded-{top|right|bottom|left}-{sm|lg}`
+ `.rounded-circle` circle
+ `.rounded-0` no radius


#### Sizing
+ `.w-{25|50|75|100|auto}` for width 25%, 50%, 75%, 100% and auto
+ `.h-{25|50|75|100|auto}` for height 25%, 50%, 75%, 100% and auto
+ `.mw-100` set the max-width with 100%
+ `.mh-100` set the max-height with 100%


## Contributing
If you're interested in contributing to Utilities CSS, please read our [CONTRIBUTING.md](https://github.com/buuug7/utilities-css/blob/master/CONTRIBUTING.md) before submitting a pull request.  