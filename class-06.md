## Object Literals
**Objects** - grpup variables and functions to make a model
 - if a variable is part of an object it is a property
 - if a fucntion is part of an object it is a method

 the **object** with its properties and methods is stored in a varibale inside {}
 
 **properties** and **methods** hava a name called a **key**
 - an object cannot have two keys with the same name
 - value of a key can be a string, number, boolean, array or another object
 - the value of a method is ***alwasys*** a function

 ### Create objects:
 -  **literal notation** (easiest and most popular)the object is the curly braces and its contents. The object is stored in a variable with what it is named. This is the **object**
    - separate each key from its value with a :
    - separate each property and methd with a comma

### Accessing objects:
1. theNameOfTheObject.nameOfThePropertyOfMethod
- **dot notation**
  - the **.** is the **member operator** 
  - the property or method on the right is a memeber of the object on the left
2. **square bracket syntax** object name['property or method];
  - this is most commonly used when the property or method has a number or special character in ts name
  - a variable is used in place of property name

  ## The DOM (Document Object Model)
 When a browser leads a webpage it stores a model in memory. Elements, atributes, and text beceom nodes in the model. 

 You can access the nodes in js individually, in multiples, or moving from one 'relative' node to another. Ex: **getElementById()**

 Nodes **represent** elements

 Once you access a node, you can work inside of it. Ex: for text node use **nodeValue** to access text inside. You can add and remove nodes also. This is **DOM manipulation**. You can get or update values with class and id attributes

 **DOM queries** are the methods that find elements in a DOM tree. You can store the ***location*** of the element that has been found with jquery, in a variable. If the script needs the variable more than once, **"caching"** it to save the browser from searching again. The variable stores the ***reference to*** the object in the DOM tree

 Queries can return one element or a collection of nodes called a **NodeList**. For those methods that have the ability to return multiple nodes, they will ***always*** return a NodeList, even if there is only one node. 
 A NodeList is similar to an array with [], but it is not an array, it is a **collection**

 **getElementById** is the fastest because Id is unique to a single element

 DOM methods can be used on other element nodes to find descendants of that node

**NodeLists** store nodes in the same order that they appear in HTML. Because the NodeList is an ***object***, it can have properties and methods. ***length** and **item()** are examples.

**live** NodeLists are updated each time script reads page, and **static** NodeLists are not. **query selector** produces static NodeLists

To select from a NodeList you can use **item()** which returns a single node from the NodeList. Specify the index number inside the (). For efficiency, check with **length** property of NodeList to see if there is anything in it. If not, the code will not execute. You use an if conditional in the query.

**Array syntax** is preferred to **item()** because it is faster.[]

YOu can select nodes by class attributes, tag names, and by CSS selectors

**querySelctor()** returns the first element that  matches CSS selector.
**querySelectorAll** reurns a NodeList of all matches of CSS selector
both these methods are only supported in more recent browesers

DOM queries dynamically change the DOM tree as script runs

You can loo though NodeLists and apply the same statements to each node. Use a for loop to go through each element. Use the counter variable inside [] to indicate which item in the NodeList is being used.

You can **traverse** the DOM once you have a node, you can select another element that's related to it.
- **parentNode**
- **previousSibling nextSibling**
- **firstChild lastChild**
Note that these selectors do not have (). They are ***properties*** of the current node, not ***methods*** to select a node. They are read-only. YOU cannot update a relative. **NOTE** most browsers treat whitespace as a tesxt node, so it is best to use jquery instead of these selectors. If the HTML has no whitespace, they can be used.

When an element contains a mix of text and other elements, you ususally work wtih the cotaining element rather that individual nodes for each descendant.

Updating the contents of an element will overwrite the intire contents of the element (text and markup)

**nodeValue** property allows you to get and edit contents. You must be on a text node, ***not the element that contains the text***
Once in the text node, you perform the change then upate the node with the change

**textContent** property allows you to collect or update ***just*** text in the element and its children

### Adding and Removing HTML Content
1. innerHTML property - faster but less secure
 - can be used on any element node
2. DOM manipulation - slower but safer
 - a set of DOM methods that creates elements and text nodes, then you can attach or remove them from tree

