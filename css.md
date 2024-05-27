# Comments

```CSS
/*This is a comment*/
```
# Colors

- Color names
- RGB Format
    >- rgb(255, 0, 255)
    >- 0 - 255 
    >- (red, green, blue)
    >-  rgb(255, 0, 0) - red --> rgb(0, 255, 0) - green --> rgb(0, 0, 255) - blue
- RGBA Format
    >- rgba(255, 0, 255, 0.5)
    >- rgb(0 - 255) --> a(0 - 1)
    >- (red, green, blue, alpha)
- Hexadecimal Format
    >- #ff6347
    >- #rrggbb -> r - red, g - green, b- blue
    >- #000000 -> black
    >- #ffffff -> white
- HSL Format
    >- hsl(245, 50%, 80%)
    >- 0 - 360, 0 - 100%, 0 - 100%
    >- hue, saturation, lightness
    >- hue -> 0 - red, 120 - green, 240 - blue
    >- saturation -> 0 - gray, 100 - full color
    >- lightness -> 0 - black, 50 - neither light or dark, 100 - white

# Font Properties

Google fonts -> select this font -> copy the link -> paste in the code -> change the font family
>- `font-family: roboto`
>- `font-style: italic`
>- `font-weight: bold`
>- `font-variant: small-caps`
>- `font-size: 25px`
>- `color: aqua`
>### Short-hand Properties
>- `font: bold 12px Arial` - Short-hand

# Background Properties

>- `background-color: yellow`
>- `background-image: url(location.jpg)`
>- `background-repeat: no-repeat`
>- `background-repeat: repeat-x` - repeats horizontally
>- `background-repeat: repeat-y` - repeats vertically
>- `background-size: 300px 250px`
>- `background-size: cover` - hint: use instead of 100%
>- `background-position: top center` - hint: change the body size
>- `background: yellow url(location.png) no-repeat` - Short-hand
>- `background-attachment: fixed` -> scroll
>- `background-origin: padding-box` -> content-box, border-box
>- `background-clip: text` -> `-webkit-background-clip: text` - hint: `color: tranparent`

# Background Gradient

>### Linear Gradient
>- `background: linear-gradient(45deg, red, yellow, orange)` -> to right, to left, to top, to bottom, to bottom right, to bottom left, to top left, to top right, 0-360 deg
>### Repeating Linear Gradinet
>- `background: repeating-linear-gradient(45deg, red, yellow 20%, orange 30%)` -> to right, to left, to top, to bottom, to bottom right, to bottom left, to top left, to top right, 0-360 deg
>### Radial Gradient
>- `background: radial-gradient(red 25%, yellow )` -> circle, closest-side at 70% 20%, farthest-side at 80% 30%, closest-corner at 20% 30%, farthest-corner at 10% 20%
>### Repeating Radial Gradient
>- `background: repeating-radial-gradient(red, yellow 10%, green 20%)` -> circle, closest-side at 70% 20%, farthest-side at 80% 30%, closest-corner at 20% 30%, farthest-corner at 10% 20%
>### Conic Gradient
>- `background: conic-gradient(from 90deg, red, yellow, green)` -> hint: `border-radius: 50%` -> at 60% 30%
>- -> To get result like Pie chart -> `background: conic-gradient(red 0deg, red 90deg, yellow 90deg, yellow 80deg, green 180deg, green 270deg, blue 270deg)`
>### Repeating Conic Gradient
>- `background: repeating-conic-gradient(red 10%, yellow 20%)` -> at 60% 30%

# Background Blend

>- `background: linear-gradient(red, yellow), url(location.jpg)` - hint: `background-size: cover`
>- `background-blend-mode: normal` -> screen, overlay, darken, hard-light, soft-light, multiply, color-burn, difference, exclusion, hue, color, saturation, luminosity

# Opacity

>- `opacity: 0.5`
>- 0 - 1

# Text Properties

>- `letter-spacing: 5px`
>- `text-decoration: underline` -> overline, line-through, none
>- `vertcal-align: sub` -> super
>- `text-transform: uppercase`
>- `text-align: justify`
>- `text-indent: 20px`
>- `line-height: 30px`

# List Properties

>- ul li -> `list-style-type: decimal` -> none, decimal-leading-zero
>- ul li -> `list-style-position: inside` -> outside - default
>- ul li -> `list-style-image: url(location.png)` - hint: 8 to 16 px

### To add image as list style
```CSS
ul li::before{
    content: '';
    display: inline-block;
    margin-right: 10px;
    margin-left: -10px;
    height: 10px;
    width: 10px;
    background-image: url(location.png);
    background-size: cover;
}
```

# Margin Properties

>- `margin-top: 10px`
>- `margin-bottom: 20px`
>- `margin-right: 10px`
>- `margin-left: 15px`
>### Short-hand Properties
>- `margin: 30px` -> all sides
>- `margin: 10px 20px 25px 15px` -> (top right bottom left)
>- `margin: 10px 20px` -> (vertical, horizontal)
>- `margin: 10px 20px 15px` -> (top, horizontal, bottom)

# Padding Properties

>- `padding-top: 10px`
>- `padding-bottom: 20px`
>- `padding-right: 10px`
>- `padding-left: 15px`
>### Short-hand Properties
>- `padding: 30px` -> all sides
>- `padding: 10px 20px 25px 15px` -> (top right bottom left)
>- `padding: 10px 20px` -> (vertical, horizontal)
>- `padding: 10px 20px 15px` -> (top, horizontal, bottom)

# Border Properties

>### Border Style
>- `border-top-style: solid`
>- `border-left-style: double`
>- `border-right-style: dotted`
>- `border-bottom-style: solid`
>### Border Color
>- `border-top-color: red`
>- `border-left-color: green`
>- `border-right-color: yellow`
>- `border-bottom-color: orange`
>### Border Width
>- `border-top-width: 10px`
>- `border-left-width: 20px`
>- `border-right-width: 15px`
>- `border-bottom-width: 25px`
>### Short-hand Properties
>- `border-style: solid`
>- `border-color: red`
>- `border-width: 5px`
>- `border: 10px solid red`
>### Border Radius
>- `border-radius: 10px`
>- `border-radius: 0px 10px 0px 20px` -> (left-top, right-top, right-bottom, left-bottom)

# Outline

>- `outline-width: 2px`
>- `outline-style: solid`
>- `outline-color: red`
>- `outline-offset: 2px` -> moves 2px away from the border
>- `outline: 2px dashed blue` -> Short-hand

# Box-Sizing

>- `box-sizing: content-box` -> adds additional dimensions to the initial dimension
>- `box-sizing: border-box` -> adjust the additional dimensions to initial dimensions

# Selectors

## Simple Selectors

### Element Selector
```CSS
                /*Select by HTML element*/
h1{
    color: red;
}
```

### ID Selector
```CSS
                /*Select by ID name*/
#name{
    color: red;
}
```

### Class Selector
```CSS
                /*Select by Class name*/
.name{
    color: red;
}
```

### Universal Selector
```CSS
                /*Style for the entire document*/
*{
    margin: 0;
}
```

## Combinators Selectors

### Decendant Selector
To style all the `p` tag inside the `div` element
```CSS
div p{
    color: blue;
}
```

### Direct Child Selector
To style all the `p` tag of direct child of `div`
```CSS
div > p{
    color: red;
}
```

### Adjacent Selector
To style the first (adjacent) `p` tag after the `div` element
```CSS
div + p{
    color: blue;
}
```

### General Sibling Selector
To style the `p` element of direct sibling of `div` element
```CSS
div ~ p{
    color: red;
}
```

## :Root Pseudo Selector

>- To style multiple elements with same property values.
>- Create a variable with any name preferred and starting with "--".
```CSS
:root{
    --bgcolor: blue;
    --color: red;
}
div{
    background-color: var(--bgcolor);
    color: var(--color);
}
```

## Pseudo Class Selectors

To style the first child of the `ul` element
```CSS
ul li:first-child{
    color: red;
}
```

To style the last child of the `ul` element
```CSS
ul li:last-child{
    color: blue;
}
```

To style the nth child of the `ul` element
```CSS
            /* n, 2n, 2n+1, ...  <->  n = 0, 1, 2, 3, .... */
ul li:nth-child(n){
    color: green;
}
```

To style the last nth child of the `ul` element
```CSS
ul li:nth-last-child(n){
    color: green;
}
```

To style the odd child of the `ul` element
```CSS
ul li:nth-child(odd){
    color: green;
}
```

To style the nth element
```CSS
p:nth-of-type(1){
    color: red;
}
```

To style the nth last element
```CSS
p:nth-last-of-type(1){
    color: red;
}
```

To style the odd element
```CSS
ul li:nth-of-type(odd){
    color: green;
}
```

To style the child element which has only one child
```CSS
li:only-child{
    color: green;
}
```

To style the element which only one time occured
```CSS
p{
    color: blue;
}
```

To style the first element 
```CSS
li:first-of-type{
    color: red;
}
```

To style the last element 
```CSS
li:last-of-type{
    color: red;
}
```

To style the empty element
```CSS
p:empty{
    border: 2px solid red;
}
```

To style the element which do not have particular value
```CSS
p:not(.box){
    color: green;
}
```

To style the particular `lang` atribute
```CSS
/* <p lang="en">content</p> */
p:lang(en){
    color: red;
}
```

### :is() Pseudo Class Selector

To style different element from same parent
```CSS
div :is(h1, p){
    color: red;
}
```

To style same element from different parents
```CSS
:is(#d1, #d2) h2{
    color: green;
}
```

To style different elements from different parents
```CSS
:is(#d1, #d2) :is(h2, p){
    color: blue;
}
```

To hover the effect using is()
```CSS
:is(#d1, #d2) h2:hover{
    color: yellow;
}
```

## Pseudo Class in Anchor Tag

To style `a` tag
```CSS
a{
    text-decoration: none;
}
```

To change the color when the mouse hovers
```CSS
a:hover{
    color: red;
}
```

To change the color when pressing
```CSS
a:active{
    color: orange;
}
```

To change the color after visited
```CSS
a:visited{
    color: green;
}
```

To style the targeted element
```HTML
<a href=#para>Para 1</a>
<p id="para">Content</p>
```
```CSS
p:target{
    background-color: green;
}
```

## Pseudo Class in Form

To style the element when it is focused
```CSS
#txt:focus{
    outline: none;
}
```

To style the `checkbox, enabled, disabled, required, read-only, read-write`
```CSS
input[type="checkbox"]:checked{
    box-shadow: 0 0 0 3px red;
}
```

To style `valid` and `invalid`
```HTML
<input type="text" placeholder= "Enter Username" pattern="[a-z]*">
```
```CSS
input[type="input"]:valid{
    border-color: gray;
}
```

To style `deafult`
```HTML
<input type="radio"checked>
<option value="apple" selected>CSS</option>
```
```CSS
input[type="radio"]:default{
    box-shadow: 0 0 0 3px red;
}

option:default{
    color: red;
}
```

## Pseudo Element Selector

To style the placeholder
```CSS
input::placeholder{
    color: green;
}
```

To style the selected content
```CSS
p::selection{
    background-color: red;
}
```

To style the first letter 
```CSS
p::first-letter{
    color: green;
}
```

To style the first line
```CSS
p::first-line{
    color: yellow;
}
```

### ::before Pseudo Element Selector

- To style before the particular content, but it will appear inside the content
- `content: ''` is must to include
- Hint: Use `position` property to style
```CSS
.box::before{
    content: '';
    width: 100%;
    height: 20px;
    background-color: red;
}
```
### ::after Pseudo Element Selector

- To style after the particular content, but it will appear inside the content
- `content: ''` is must to include
- Hint: Use `position` property to style
```CSS
.box::after{
    content: '';
    width: 100%;
    height: 20px;
    background-color: red;
}
```

## Selector Style Preference

>- ID first priority
>- Class second priority
>- Element third priority

### To break the rule
```CSS
p{
    color: red !important;
}
```

# More Selectors Properties

To select multiple Selectors with same property and value.
```CSS
h1, p{
    color: red;
}
```







To style all the element with same attribute
```CSS
div[class]{
    background-color: yellow;
}
```

To style particular element with atribute value
```CSS
div[class="box"]{
    color: red;
}
```

To style the element with attribute even if other class name has specific style
```CSS
/*  <div class="box txt"> </div>  */
div[class~="box"]{
    color: red;
}
.txt{
    color: green;
}
```

To style the element with attribute starting value
```CSS
/*  <a href="test.png> </a> */
a[href^="test"]{
    color: red;
}
```

To style the element with attribute ending value
```CSS
/*  <a href="test.png> </a>  */
a[href="png"]{
    color: blue;
}
```

# Display Properties

>- `display: block` -> Takes the width of parent element
>- `display: none` -> Hides the content
>- `display: inline` -> Acts as inline and, width and height can be assigned
>- `display: inline` -> Acts as inline element

### To change the list items to single line
```CSS
ul li{
    display: inline;
    list-style-type: none;
    background-color: orange;
    margin-left: 15px;
    padding: 10px;
}
```

# Display Table Properties

>- `display: table`
>- `display: table-row`
>- `display: table-cell`
>- `display: table-header-group`
>- `display: table-footer-group`
>- `display: table-caption`
>- `display: table-column-group`
>- `display: table-column`
>- `display: table-row-group`

### To display table without `table` element

```HTML
<body>
    <div class="table">
        <div class="caption">For Practicing</div>        
        <div class="col-group">
            <div class="table-col col-1">1</div>
            <div class="table-col col-2">2</div>
            <div class="table-col col-3">3</div>
        </div>
        <div class="header">
            <div class="row">
                <div class="col">Name</div>
                <div class="col">Age</div>
                <div class="col">City</div>
            </div>
        </div>
        <div class="row-group">
            <div class="row">
                <div class="col">Jack</div>
                <div class="col">22</div>
                <div class="col">Chennai</div>
            </div>
            <div class="row">
                <div class="col">Sam</div>
                <div class="col">28</div>
                <div class="col">Mumbai</div>
            </div>  
        </div>    
        <div class="footer">
            <div class="row">
                <div class="col">Total</div>
                <div class="col"></div>
                <div class="col">5</div>
            </div>
        </div>   
    </div>
</body>
```
```CSS
.table{
    display: table;
    width: 600px;
}
.row{
    display: table-row;
}
.col{
    display: table-cell;
    border: 2px solid orangered;
    padding: 10px;
    text-align: center;
}
.header{
    display: table-header-group;
    font-weight: bold;
    text-align: center;
    background-color: orangered;
    color: white;
}
.footer{
    display: table-footer-group;
}
.caption{
    display: table-caption;
    text-align: center;
    color: orangered;
    font: bold 32px Arial;
}
.col-group{
    display: table-column-group;
}
.table-col{
    display: table-column;
}
.col-2{
    width: 80px;
    background-color: yellow;
}
.row-group{
    display: table-row-group;
    color: blue;
}
```

# Box Shadow

>- `box-shadow: 10px 8px 5px 0px rgba(0, 0, 0, 0.8)` -> (horizontal offset, vertical offset, blur radius, spread)
>- lower the blur radius gives solid border

# Creating a Chess Board

```HTML
<body>
    <div class="table">
        <div class="caption">Chess Board</div>
        <div class="row-group">
            <div class="row row1">
                <div class="col">&#9814</div>
                <div class="col">&#9816</div>
                <div class="col">&#9815</div>
                <div class="col">&#9812</div>
                <div class="col">&#9813</div>
                <div class="col">&#9815</div>
                <div class="col">&#9816</div>
                <div class="col">&#9814</div>
            </div>
            <div class="row row2">
                <div class="col">&#9817</div>
                <div class="col">&#9817</div>
                <div class="col">&#9817</div>
                <div class="col">&#9817</div>
                <div class="col">&#9817</div>
                <div class="col">&#9817</div>
                <div class="col">&#9817</div>
                <div class="col">&#9817</div>
            </div>
            <div class="row row3">
                <div class="col"></div>
                <div class="col"></div>
                <div class="col"></div>
                <div class="col"></div>
                <div class="col"></div>
                <div class="col"></div>
                <div class="col"></div>
                <div class="col"></div>
            </div>
            <div class="row row4">
                <div class="col"></div>
                <div class="col"></div>
                <div class="col"></div>
                <div class="col"></div>
                <div class="col"></div>
                <div class="col"></div>
                <div class="col"></div>
                <div class="col"></div>
            </div>
            <div class="row row5">
                <div class="col"></div>
                <div class="col"></div>
                <div class="col"></div>
                <div class="col"></div>
                <div class="col"></div>
                <div class="col"></div>
                <div class="col"></div>
                <div class="col"></div>
            </div>
            <div class="row row6">
                <div class="col"></div>
                <div class="col"></div>
                <div class="col"></div>
                <div class="col"></div>
                <div class="col"></div>
                <div class="col"></div>
                <div class="col"></div>
                <div class="col"></div>
            </div>
            <div class="row row7">
                <div class="col">&#9823</div>
                <div class="col">&#9823</div>
                <div class="col">&#9823</div>
                <div class="col">&#9823</div>
                <div class="col">&#9823</div>
                <div class="col">&#9823</div>
                <div class="col">&#9823</div>
                <div class="col">&#9823</div>
            </div>
            <div class="row row8">
                <div class="col">&#9820</div>
                <div class="col">&#9822</div>
                <div class="col">&#9821</div>
                <div class="col">&#9818</div>
                <div class="col">&#9819</div>
                <div class="col">&#9821</div>
                <div class="col">&#9822</div>
                <div class="col">&#9820</div>
            </div>
        </div>
    </div>
</body>
```

```CSS
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
body{
    background: repeating-conic-gradient(at 10% 10%, #593954, #013440 5%, #026873 10%);
    background-size: cover;
    background-attachment: fixed;
}
.table{
    display: table;

    margin: auto;
    padding: 1.5vw;
    border: 0.1vw solid white;
    background: repeating-conic-gradient(#593954, #013440 5%, #026873 10%);
    border-radius: 5%;
}
.row{
    display: table-row;
}
.col{
    display: table-cell;
    border: 0.1vw solid black;
    background-color: white;
    font-size: 3vw;
    text-align: center;
    align-content: center;
    width: 5vw;
    height: 5vw;
}
.row-group{
    display: table-row-group;
}
.caption{
    display: table-caption;
    text-align: center;
    color: purple;
    font: bold 2vw Arial;
    border-radius: 10%;
}
.row1 .col:nth-child(even),
.row2 .col:nth-child(odd),
.row3 .col:nth-child(even),
.row4 .col:nth-child(odd),
.row5 .col:nth-child(even),
.row6 .col:nth-child(odd),
.row7 .col:nth-child(even),
.row8 .col:nth-child(odd){
    background-color: #038C7F;
}
.col:hover{
    font-size: 3.5vw;
    color: purple;
    cursor: pointer;
}
```

# Position Properties

## Static

>- `position: static` -> Default position

## Relative

>- Same as static position, but has 4 properties -> left, right, top, bottom
```CSS
div{
    position: relative;
    left: 20px;
}
```

## Absolute

>- Takes the element outside of the document flow
>- Properties used -> left, right, top, bottom, relative
>- Use the relative property to position the child element to move along inside the parent element
```CSS
.parent{
    position: relative;
}
.child{
    position: absolute;
    right: 0;
}
```

## Fixed

>- Takes the element out of the document flow
>- Properties used -> left, right, top, bottom
```CSS
div{
    positon: fixed;
    right: 0;
}
```

## Sticky

>- Used to stick the element in the particular position even after scrolling
```CSS
.nav{
    position: sticky;
    top: 0;
}
```

# Z index Property

-> The greater the number of value will be on the top
```CSS
div{
    position: absolute;
    z-index: 1;
}
```

# Min-height & Max-height Properties

>- `min-height: 200px` -> minimum height will be 200px as initial stage and it can be automatically expanded if the content needs more space.
>- `max-height: 200px` -> height will be based on the content and can be expanded upto maximum of 200px.

# Min-width & Max-width Properties

>- It is used mostly in images, because text will automatically wrap the content.
>- `min-width: 500px` -> minimum width will be 500px as initial stage and it can be automatically expanded if the content needs more space.
>- `max-width: 500px` -> width will be based on the content and can be expanded upto maximum of 500px.
```CSS
div{
    max-width: 500px;
}
img{
    width: 100%;
}
```

# Overflow Property

>- `overflow: visible` -> default
>- `overflow: hidden` -> hides the overflow content
>- `overflow: scroll` -> adds a scroll bar for both horizontal and vertical
>- `overflow: auto` -> adds a scroll bar for specific need
>- `overflow-x: scroll` -> adds a scroll bar for x-axis
>- `overflow-y: scroll` -> adds a scroll bar for y-axis

# Column Property

### Column
>- `column-count: 2` -> adds 2 columns
>- `column-width: 150px` -> adds 150px to each columns
>- `column-gap: 50px` -> adds 50px gap between the columns

### Column-rule -> adds a line between the columns
>-  `column-rule-style: solid`
>-  `column-rule-width: 2px`
>-  `column-rule-color: red`
>- `column-rule: 2px solid red` -> Short-hand

### Column-span
>- `column-span: none` -> default
>- `column-span: all` -> removes particular element from the column

# Units

Commonly used units: `px, %, em, rem, vw, vh, vmax, vmin`

## Absolute Units
> Fixed Size for all type of screens
>- cm -> Centimeter
>- mm -> Millimeter
>- in -> Inch
>- px -> Pixels
>- pt -> Points
>- pc -> Picas

## Relative Units
> Size depends on parents
>- em ->  `1 em = 16px` -> browser default size -> works based on direct parent
>- rem -> root em -> works based on the root element `html` or browser default
>- ch
>- ex
>- vw -> Viewport Width -> works based on device width
>- vh -> Viewport Height -> works based on device height
>- vmax -> Viewport Maximum -> works based on maximum viewport value 
>- vmin -> Viewport Min imum viewport value
>- % -> Percentage -> works based on the parent size

# Transition

>- `transition-property` -> selects the property
>- `transition-duration` -> time taken to make the change
>- `transition-timing-function` -> mode of change
>- `transition-delay` -> time taken to begin the change
>- `transition` -> Short-hand

### Transition-Timing-Function

>- `ease` -> Starts slow - Fast - Ends Slow
>- `linear` -> Maintain same speed
>- `ease-in` -> Slow Start
>- `ease-out` -> Slow End
>- `Ease-in-out` -> Slow Start and Slow End
>- `steps(6)` -> Changes step by step
>- `cubic-bezier(.17, .67, .83, .67)` -> Manual change -> Go to the website Cubic Bezier

```CSS
div{
    width: 300px;
    height: 300px;
    background-color: red;
    transition-property: width, height, background-color;
    transition-duration: 0.5s, 0.5s, 0.5s;
    transition-timing-function: linear;
    transition-delay: 0.5s;

}
div:hover{
    width: 600px;
    height: 600px;
    background-color: yellow;
}
```

Short-hand
```CSS
div{
    transition-property: all;
    transition-duration: 0.5s;
    transition-timing-function: ease-in-out;
    transition-delay: 0.5s;
}
```
```CSS
div{
    transition: all 0.5s ease-in 1s;
}
```

# Flex Box

>- `display: flex` -> set this to the parent
>- The child will automatically change to flex items

## Main Axis and Cross Axis

>- Main Axis is X-axis
>- Cross Axix is Y-axis

## Flex Direction

>- `flex-direction: row` -> Default
>- `flex-direction: row-reverse` -> Reverese the row
>- `flex-direction: column` -> alignment will be in columns
>- `flex-direction: column-reverse` -> alignment will be in reversed columns

## Flex Wrap

>- `flex-wrap: nowrap` -> Default
>- `flex-wrap: wrap` -> Stops the overflow
>- `flex-wrap: wrap-reverse` -> Reverses the wrapping process

## Justify Content -> Main Axis

>- `justify-content: flex-start` - Default
>- `justify-content: flex-end` - Right align the content
>- `justify-content: center` - Center align the content
>- `justify-content: space-between` - Assign equal space between the content
>- `justify-content: space-around` - Assign equal space around the content

## Align Content -> Cross Axis

>- `align-content: flex-start` -> Default
>- `align-content: flex-end` -> Align to the bottom
>- `align-content: center` -> Align to the center
>- `align-content: space-between` - Assign equal space between the content
>- `align-content: space-around` -> Assign equal space around the content
>- `align-content: centbaselineer` -> Align to the content with different sizes to same baseline
>- `align-content: stretch` -> Stretches the content to maximum height

## Flex Order

To change the order of the elements
```CSS
.box:nth-child(2){
    order: 3;
}
```

## Align Self

To align individual flex items

>- `align-self: stretch` -> maximize the content size
>- `align-self: flex-start` -> align to the top
>- `align-self: flex-end` -> align to the bottom
>- `align-self: center` -> align to the center

```CSS
.box:nth-child(2){
    align-self: center;
}
```

## Flex Grow

To enlarge a particular flex item with the ratio amount
```CSS
.box:nth-child(2){
    flex-grow: 2;
}
```

## Flex Shrink

To shrink a particular flex item with the ratio amount
```CSS
.box:nth-child(2){
    flex-shrink: 2;
}
```

# Creating Navigation Bar using Flex Box

## Simple Navigation Bar

```HTML
<body>
    <header>
        <h2 class="logo">Little Lemon</h2>
        <nav>
            <ul class="nav-link">
                <li><a href="#">Home</a></li>
                <li><a href="#">Product</a></li>
                <li><a href="#">Pricing</a></li>
                <li><a href="#">Services</a></li>
            </ul>
        </nav>
        <button>Contact Us</button>
    </header>
</body>
```

```CSS
*{
    font-family: Arial, Helvetica, sans-serif;
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}
header{
    display: flex;
    justify-content: flex-end;
    align-items: center;
    padding: 15px 3%;
    background-color: darkcyan;
}
.logo{
    cursor: pointer;
    color: white;
    font-variant: small-caps;
    font-weight: 400;
    margin-right: auto;
}
.nav-link{
    list-style: none;
    display: flex;
}
.nav-link li a{
    color: white;
    text-decoration: none;
    padding: 10px;
    transition: all 0.3s linear;
}
.nav-link li a:hover{
    color: black;
    background-color: aquamarine;
}
button{
    padding: 5px 25px;
    margin-left: 10px;
    background-color: rgb(0, 216, 173);
    border: none;
    color: white;
    border-radius: 50px;
    cursor: pointer;
}
button:hover{
    background-color: rgba(0, 216, 173, 0.8);
}
```

## Animated Simple Navigation Bar

```HTML
<body>
    <header>
        <nav>
            <ul class="nav-link">
                <li><a href="#">Home</a></li>
                <li><a href="#">Product</a></li>
                <li><a href="#">About</a></li>
                <li><a href="#">Contact Us</a></li>
            </ul>
        </nav>
    </header>
</body>
```

```CSS
*{
    padding: 0;
    margin: 0;
    box-sizing: border-box;
}
body{
    font-family: Arial, Helvetica, sans-serif;
}
nav{
    position: relative;
    top: 20vw;
    text-align: center;
}
nav ul{
    display: inline-block;
    list-style: none;
    transform: skew(-25deg);
}
.nav-link li{
    font-variant: small-caps;
    font-weight: 540;
    background-color: teal;
    color: white;
    float: left;
    border-right: 2px solid white;
    box-shadow: 3px 3px 3px rgba(0,0,0,0.8);
    transition: all 0.3s linear;
}
.nav-link li:last-child{
    border: none;
    border-radius: 0 7px 7px 0;
}
.nav-link li:first-child{
    border-radius: 7px 0 0 7px;
}
.nav-link li a{    
    padding: 10px 20px;
    text-decoration: none;
    color: inherit;
    display: block;
    transform: skew(25deg);
}
.nav-link li:hover{
    background-color: black;
}
```

## Responsive Navigation Bar

```HTML
<body>
    <div class="navbar">
        <div class="logo">Little Lemon</div>
        <a href="#" class="btn">
            <span class="bar"></span>
            <span class="bar"></span>
            <span class="bar"></span>
        </a>        
        <div class="nav-links">
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">Product</a></li>
                <li><a href="#">About</a></li>
                <li><a href="#">Contact Us</a></li>
            </ul>
        </div>
    </div>
    <script src="script.js"></script>
</body>
```

```CSS
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, Helvetica, sans-serif;
}
.navbar{
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: #2c3e50;
    color: white;
}
.logo{
    font-size: 25px;
    font-weight: 500;
    margin: 10px;
    font-variant: small-caps;
}
.nav-links ul{
    display: flex;
}
.nav-links ul li{
    list-style: none;
}
.nav-links li a{
    color: inherit;
    text-decoration: none;
    display: block;
    padding: 16px;
}
.nav-links ul li:hover{
    background-color: #34495e;
}
.btn{
    position: absolute;
    top: 16px;
    right: 16px;
    width: 30px;
    height: 22px;
    display: none;
    flex-direction: column;
    justify-content: space-between;
}
.bar{
    width: 100%;
    height: 3px;
    background-color: white;
}

@media (max-width:600px){
    .btn{
        display: flex;
        left: 16px;
    }
    .nav-links{
        display: none;
        width: 100%;
    }
    .navbar{
        flex-direction: column;
        align-items: flex-end;
    }
    .nav-links ul{
        flex-direction: column;
        width: 100%;
    }
    .nav-links ul li{
        text-align: left;
    }
    .nav-links.active{
        display: flex;
    }
}
```

```JS
const btn = document.getElementsByClassName('btn')[0];
const navbar = document.getElementsByClassName('nav-links')[0];
btn.addEventListener('click', change);
function change(){
    navbar.classList.toggle('active')
}
```

