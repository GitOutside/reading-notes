## Lists
There are two types of lists in HTML. Unordered and Ordered, which use the ```<ol>``` anf ```<ul>``` tags, respectively. 

Browsers indent lists, by default. You can style the numbers and bullets for the two lists with CSS.

```<dl>``` the definition list contains a series of terms and their definitions. 
Inside the ```<dl>``` are the ```<dt>``` and ```<dd>``` for definied term and the actual definiions, respectively.
 
You can nest lists, and the browser will indent the sub-lists

## Boxes
Each element in HTML has an invisible box around it. Using CSS, the boxes can be manipulated.

### Dimensions for boxes
- pixels
- %
  - size of thebox is based on the size of its container.
- ems
  - size is based on the size of text within it
  - useful for designing for multiple screen types 

To make sure that content is readable despite different screen sizes, you can limit the height and width of the boxes, using ```<min-width>```, ```<max-width> `` and their height counterparts.

if a box is not big enough, you can control the "extra" content with the **overflow** property. This property tells the browser what to do with it. 
- hidden
- scroll

Each box has 3 properties that can be adjusted:
1. Border 
 - the edge of the box
2. Margin
 - sits outside the border
3. Padding
 - the space between the border and the conten

 **border-width** thin, thick, or medium. No percentages.

 can control each side with its owm property:
 - top
 - right
 - bottom
 - left

 ex: **border-width**: 2px, 1px, 1px, 2px;

 You can also **border-style** with these values:
 - solid
 - dotted
 - dashed
 - groove
 - ridge
 - inset
 - outset
 - hidden/none
 also can do each side diff. with **border-top-style** right, left, bottom

 **border-color** ca nuse RGB, hex, or names

 can do each side separate just like style and width.
 There is also a shorthand, whic combines width, style, and color
 **border**: 3px dotted #0055gg;

 Can do the same with paddng and margin

 ### Centering Content
 set **left-margin** and **right-margin** to auto
 You must set a width or else it will span the entire page. This is inherited by child elements

 You can convert an inline to block and vice-versa. It also can hide an element.
 **inine**
 **block**
 **inline-block** flows like an inline element, but keeps block features
 **none**

 **visibility** can be hidden or visible. 
 If hidden, there will be a space where the hidden element resides- use **display: none** to avoid this.


 **border-image**
 -requires
  1. URL of image
  2. where to put image
  3. **stretch**, **repeat**, or **reound**. Needs **border-width** for image to be shown

  **box-shadow**
  ***horzontal offset*** neg values position to left
  ***vertical offset*** neg values position to the top
  ***Blur distance*** if omitted, shadow is solid line
  ***spread of shadow*** positive value expands

  **border-radius** for rounded corners. Can also do each side separately. Can use shorthand

  ## Js Decisions and Loops
  **if else** checks condition. If **TRUE** first code executed. If **FALSE** second code executed. 
  - statements inside **if else** need semi-colon, but not after curly brace

  **switch** is assigned a value. Inside curly braces are **cases** that list possible values and the code that needs to run if matched. Each **case** is followed by **break** that, when run, tells computer to end **switch** and move to next code.
  - has deafult setting

JavaScript uses **weak typing** which means it can change data types to complete an operation. This is **type coercion**.
To avoid unexpected values, always use === and !== rather than == and !=

## Truthy and Falsy
caused by type coercion
everything can be treated as true or false
**Falsy** values - false or **0**
                 - 0
                 - ''
                 - NaN
                 - var with no value assigned

Most everything else is truthy or **1**