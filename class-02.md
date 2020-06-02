# HTML 
- Structural markup
  - describes 
- Semantic markup
  - doesn't change the structure. only for information
  - used for screen readers and search engines
 
Examples: 
```<stong>``` and ```<em>``` are used for bolded and italicized text
```<blockquote>``` and ```<q>``` for long, block and short, inline quotes
```<abbr>``` abbreviation
```<cite>``` citation 
```<dfn>``` defining a new term
```<address>``` contact info for page author
```<ins>``` shows inserted text, usually underlined
```<del>``` deleted text, usually has line through it
```<s>``` is also text with a line through it, but not to indicate edit. To show a change that is no longer accurate or relevant. think sale price

# CSS
The **key** to CSS is to imagine that every element defined in HTML has a box around it. That's what you style with CSS.

Two parts to CSS rules 
1. selector - which element to style
2. declaration - how the selction is styled. 
    - Inside the ```{}```
    - two parts - property and value, separated by a ```:```

```<link>``` in in HTML and it is where to tell the browser to sind CSS file. Has three attributes:
  1. **href** specifies path for CSS
  2. **type** self-explanatory. Should be ```"text/css"```
  3. **rel** relationship of HTML to linked file. For CSS is ```"***stylesheet***"```
  can use multiple stylesheets for big projects

  Can place CSS inside HTML using ```<style>``` which is in ```<head>```.
One attribute ***type*** is ```"text/css"```

- CSS selectors are case sentitive
- Must match exactly
- many types of selectors for specific elements

### CSS Cascade Rules
1. if two selectors are the same, the latter trumps previous
2. the more specific selector trumps less specific
3. you can add ```! important``` to make something trump all other rules for element

Some properties are inherited by child elements, but not all.
You can force inheritance with ***inherit*** for the value of a property

Using a separate style sheet has advantages.
- all pages of a site can use one stylesheet. Fewer and faster edits
- page loads faster
- makes HTML eaasier to read

Can put CSS in HTML, but best to limit that to pages with rules that differ from the rest of the site.

Test new sites on different browsers. CSS3 is newest iteration

### JavaScript
**Script** is a set of instructins for computer.
Each step is s statement.
- each statement starts on a new line and ends with ```;```
Code blocks in ```{}```
Case sensitive
Should write comments in js to explain what it does
Comments with ```/* */``` for multi line or ```//``` for single line

**variables** store bits of data temporarily. Remembering them

Must declare a variable by **var xyz = blah**

**var** is a keyword so it js interprets it
**identifier** is what it sounds like
```(use camel case for more than one word)```. Should be descriptive
```=``` means assign not equal

**data types**
number
string - inside single or double quotes
 - you can use quotes inside a string, but you must use the opposite type to enclose the string. OR you can use ```\``` **before** each quotation mark in a string
boolean - T or F

There are shorthand ways to write variables. It makes code a little harder to read

Once a variable has been declared, you can change it just by changing what it has been assigned

### 6 Rules for Naming Variables
1. Must begin with a letter, ```$```, or _. Cannot start with a number
2. Can contain letters, numbers, _, or ```$```. Do not use -
3. Cannot use keywords or reserved words
4. case sensitive. Do not name two var the same name with only diff case
5. Use descriptive name
6. camelCase

Arrays store lists of values, enclosed in ```[]```
- Can add new values to an array because you do not have to specify how many values there are.
- Separate values with commas
- values do not have to be same type
- array constuctor is a less-favored alternative
- arrays start at 0, not 1

to recall a value from an array :
 var xyz; xyz = abc ```[1]```;
 the name of the array followed by ```.```length tells n=how many values in array

 you can change a value in an array by accessing it like this:
 abc[2] = 'blah'

 ### Expresssions
 two types:
 1. assigning a value
 2. use two or more values to return a single value. numbers or strings

 ### Operators
 allow programmers to create one value from multiple
   - ```=``` assignment
   - math
   - strings
   - comparison
   - logical

Order of operators
Parenthesis
Mult/Div
Add/Sub
  
## Evaluations, Decisions, Loops
flowcharts can help plan where decisions are made about which code to run

to determine which path to take at a decision point, you set a condition, and if it returns T or F determines which path is taken.

Two components to a decision:
1. Evaluate a condition
  - compare two values. T or F
2. State what to do in given situation
  - if/else 

```==``` is equal to
```!=``` is not equal to
```===``` strict equal to. same value and type
```!==``` strict not equal to. both value and type ***not*** the same
```>, <, >=, and <=```

you can compare variables, and expressions

### Logical Operators
compare the results of more than one comparison operator.
```&&``` both must be true to return true
```||``` both must be fale to return false
```!``` inverts a single boolean to opposite

- evaluated left to right

**IF** statements check a condition. If condition returns T, code is executed. If F, code not executed, continues to next line after coe block

**IF/ELSE** statements check a condition. If condition returns T, first code block is executed. If condition returns F, the second code block of code is run.