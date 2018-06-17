# Utility CSS

Simple and easy to use utility CSS, inspired by [tailwindcss](https://github.com/tailwindcss/tailwindcss), but the tailwindcss is more complex and verbose to use. This only focused on wrap the most common use css into class name. this also compatibility with bootstrap utilities.  

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
<link href="https://cdn.jsdelivr.net/npm/utility-css/dist/utility-css.min.css" rel="stylesheet">
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

## Contributing
If you're interested in contributing to Utility CSS, please read our [CONTRIBUTING.md](https://github.com/buuug7/utility-css/blob/master/CONTRIBUTING.md) before submitting a pull request.  