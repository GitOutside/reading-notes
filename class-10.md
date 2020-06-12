#Debugging
Fiding errors

Every statement is in one of three contexts:
1. **Global** in the script, not in a fxn.
2. **Function** 
3. **Eval** 

Stacking is the way the interpreter makes its ToDo list. When a function is needed to provide data to a statement, the function goes on the stack. Then the interpreter goes on.

**every new function on stack = new execution context.**
In execution, the stacked functions work top down, returning values to where they go
two phases:
1. **prepare**: new scope created .
- variables, fxns, arguments created
2. **execute**: assign values to variables
- run fxn code and execute statements.

Each context has its own variables object. The context can access its parent's variables object. But it is best to create local variables.

So, ouer functions add to inner functions' variables, but not the other way around.

When there is an error in the script, you get an **exception**. Interp. stops and looks for handler code.
This is the way uses know what is wrong.

Whenthe interpreter sees an error, it looks in the cuurent context for a handler, if none, it goes back up chain looking for one. If none found by the time it gets to glocal context, it stops and creates **error** object. IN CONSOLE

### Error objects ```(```7 types```)```
- contains these properties:
  - name
  - message
  - fileNumber
  - lineNumber

### Dealing with errors
1. Debug
2. Handle errors 

Where is the problem?
What is the problem?
Use the console log!
Take notes!
Look at the problem in a different browser
The console log writes out what values the interpreter holds for.
- use for every step that you want to see the value for

There are different types of console methods.
1. **.info** 
2. **.warn** 
3. **.error** 
4. **.group** and **.groupEnd**
5. **.table** objects and arrays 
6. **.assert** test if condition is met

Breakpoints allow you to pause the script on any line. Then you can examine the line by hovering over any variable to see its value at that time.
Setting multiple breakpoints allows you to step through them one by one. When the debugger comes across a function, it moves onto next line after function. It steps over where the function is defined. You can tell the debugger to step into a function.
You can set conditional breakpoints, using existing variables

**try catch finally**
try to execute
catch exceptions if thrown when tried
runs either way

You can throw your own errors when you know something might cause a problem, before the interpreter sees them. This helps to "hold" erros that you anticipate so they don't break code that you want to test. 
**I need clarification on this from Nich**