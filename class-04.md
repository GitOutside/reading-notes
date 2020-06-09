## Links
use  ```<a>```. Anything between the opening and closing tags can be clicked on.
```<a href="link URL">TEXT USER CLICKS ON</a>```
 - use descriptive text for link. Be specific so when user is looking for page they are linking to, they can find it more easily
 - make links clearly visible

**href** attribute is assigned value of URL for link
  - Can be absolute (on web) or relative (within site) URL

## Directory Structure
**root folder** - top level folder. All other files and folders for site here
home page for entire sie is in index.html in root folder and that is the default if no file name is specified in URL

**URL frelative links types**
 - same folder:  ***file name***
 - child folder: ***child folder name/ file name***
 - grandchild folder: ***child folder name/grandchild folder name/file name***
 - parent folder: ***../file name***
 - grandparent folder: ***../../file name***
 
 ### ```<a>``` attributes
**href = "mailto:abc@example.com"** for use in ```<a>```to send email to link address
**target** opens the link in a new window. target="_blank". Avoid opening in new window, but if you do, inform user

to link to a spot on the same page, assign id to tag where link will go. Then in ```<a>``` tag, **href** will be assigned to the id for that spot.
```<a href="URL#id></a>```

## CSS Layout
Each HTML element is in its own box

**Block level elements**
 - start on new line
 - ```<h1>, <p>, <ul>. <li>```

 **Inline elements**
 - flow in between surrounding text
 - ```<img>, <b>

 you can set the width of each box to control the size
 separate boxes with M, B, P

 Parentage hierarchy like directories

 **3 positioning schemes to control layout**. Use **position** property
 1. normal flow
  - every block level on new line
  - 'stacks' them down page, **eve if** there is space for them to sit   side-by-side. This is default, but you can change it
  2. relative positioning
   - moves element to a position relative to normal flow
   - does not affect position of surrounding elements
   - use **position: relative; top or bottom** for vertical movement
   - use **position: relative: left or right** for horizontal movement

   ex: **p.example {**
     **position: relative;**
     **top: 15px;**
     **left: 20px;}**
   would move the element ***down*** 15px ***from*** the top, and 20px ***right, from*** the left
  3. absoulte positioning
   - positions element relative to its parent element
   - taken out of normal flow- other elements act like its not there
   - 

  

## Functions

Functions store the code to run a specific task inside {}
Name the function so it can be called upon later to run. If the function does not have a name, it will be run as soon as the browser sees it
Parameters are used like variables in the function

If a function has parameters, you have to specify them when you call it in (). (arguments)
**arguments** can be (values, etc) or (canBeVariables, etc)

Functions can return a single function, or an array of values
