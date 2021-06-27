# ANONYMOUS FUNCTIONS & FUNCTION EXPRESSIONS 
Expressions produce a value. They can be used where values are expected.
If a function is placed where a browser expects to see an expression,
(e.g., as an argument to a function), then it gets treated as an expression.

# FUNCTION DECLARATION
A function declaration creates a function that you can call later in your code. It is the type of function
you have seen so far in this book.
In order to call the function later in your code, you must give it a name, so these are known as named
functions. Below, a function called area() is declared, which can then be called using its name.

# FUNCTION EXPRESSION
If you put a function where the interpreter would expect to see an expression, then it is treated as an
expression, and it is known as a function expression.
In function expressions, the name is usually omitted.
A function with no name is called an anonymous function. Below, the function is stored in a variable
called area. It can be called like any function created with a function declaration

# IMMEDIATELY INVOKED FUNCTION EXPRESSIONS 
This way of writing a function is used in several different situations.
Often functions are used to ensure that the variable names do not conflict with each other (especially if the page uses more than one script).

# IMMEDIATELY INVOKED FUNCTION EXPRESSIONS (llFE
Pronounced "iffy," these functions are not given a name. Instead, they are executed once as the
interpreter comes across them.
Below, the variable called area will hold the value returned from the function (rather than storing the
function itself so that it can be called later). 


# VARIABLE SCOPE 
The location where you declare a variable will affect where it can be used within your code. If you declare it within a function, it can only be used within that function. This is known as the variable's scope.

# LOCAL VARIABLES
When a variable is created inside a function using the var keyword, it can only be used in that function.
It is called a local variable or function-level variable.
It is said to have local scope or function-level scope.
It cannot be accessed outside of the function in which it was declared. Below, area is a local variable.
The interpreter creates local variables when the function is run, and removes them as soon as the
function has finished its task. This means that:
• If the function runs twice, the variable can have different values each time.
• Two different functions can use variables with the same name without any kind of naming conflic


# GLOBAL VARIABLES
If you create a variable outside of a function, then it can be used anywhere within the script. It is called a
global variable and has global scope. In the example shown, wa 11 Size is a global variable.
Global variables are stored in memory for as long as the web page is loaded into the web browser.
This means they take up more memory than local variables, and it also increases the risk of naming
conflicts (see next page). For these reasons, you should use local variables wherever possible. 


# USING WHILE LOOPS 
Here is an example of awhil e loop. It writes out the 5 times table. Each time the loop is run,
another calculation is written into the variable called msg.
This loop will continue to run for as long as the condition in the parentheses is true. That
condition is a counter indicating that, as long as the variable i remains less than 10, the
statements in the subsequent code block should run.

# USING DO WHILE LOOPS
The key difference between a whi 1 e loop and a do whi 1 e loop is that the statements in
the code block come before the condition. This means that those statements are run once whether
or not the condition is met.
If you take a look at the condition, it is checking that the value of the variable called i is
less than 1, but that variable has already been set to a value of 1. 

# SUMMARY
1- Conditional statements allow your code to make decisions about what to do next.
2- Comparison operators (===, ! ==, ==, ! =, <, >, <=, =>) are used to compare two operands.
3- Logical operators allow you to combine more than oneMset of comparison operators.
4- if ... else statements allow you to run one set of code if a condition is true, and another if it is false.
5- switch statements allow you to compare a value against possible outcomes (and also provides a default
option if none match).
6- Data types can be coerced from one type to another.
7- All values evaluate to either truthy or falsy.
8- There are three types of loop: for, while, and do ... while. Each repeats a set of statements. 

# The Document Object Mode
The Document Object Model (DOM) specifies how browsers should create a model of an HTML
page and how JavaScript can access and update the contents of a web page while it is in the browser window.
The DOM is neither part of HTML, nor part of JavaScript; it is a separate set of rules.
It is implemented by all major browser makers, and covers two primary areas:

# MAKING A MODEL OF THE HTM L PAGE
When the browser loads a web page, it creates a model of the page in memory.
The DOM specifies the way in which the browser should structure this model using a DOM tree.
The DOM is called an object model because the model (the DOM tree) is made of objects.
Each object represents a different part of the page loaded in the browser window.
s DOCUMENT OBJECT MODEL

# ACCESSING AND CHANGING THE HTML PAGE
The DOM also defines methods and properties to access and update each object in this model,  which in turn updates what the user sees in the browser.
You will hear people call the DOM an Application Programming Interface (API).
User interfaces let humans interact with programs; APls let programs (and scripts) talk to each other. The DOM states what your script can "ask the browser about the current page, and how to tell the browser
to update what is being shown to the user.

# WORKING WITH THE DOM TREE
Accessing and updating the DOM tree involves two steps:
1: Locate the node that represents the element you want to work with.
2: Use its text content, child elements, and attributes. 

# ACCESSING ELEMENTS
DOM queries may return one element, or they may return a Nodelist, which is a collection of nodes.
Sometimes you will just want to access one individual element (or a fragment of the page that
is stored within that one element). Other times you may want to select a group of element s, for example,
every <hl> element in the page or every <1 i> element within a particular list. 


Here, the DOM tree shows the body of the page of the list example. We focus on accessing elements
first so it only shows element nodes. The diagrams in the coming pages highlight which elements a
DOM query would return. (Remember, element nodes are the DOM representation of an element.)

# NODELISTS: DOM QUERIES THAT RETURN MORE THAN ONE ELEMENT
A Nodelist is a collection of element nodes. Each node is given an index number (a number that starts
at zero, just like an array).
The order in which the element nodes are stored in a Node List is the same order that they appeared in the
HTML page.
When a DOM query returns a Nodelist, you may want to:
• Select one element from the NodeList.
• Loop through each item in the Nodelist and
perform the same statements on each of the element nodes.
Nodelists look like arrays and are numbered like arrays, but they are not actually arrays; they are a
type of object called a collection.
Like any other object, a Nodelist has properties and methods, notably:
• The l ength property tells you how many items are in the Nodelist.
• The i tern() method returns a specific node from the Nodelist when you tell it the index number
of the item that you want (in the parentheses).
However, it is more common to use array syntax (with square_brackets) to retrieve an item from a
Nodelist (as you will see on p199). 

# SELECTI NG ELEMENTS USING CLASS ATTRIBUTES 
The get El ementsByCl ass Name() method allows you to select elements whose c 1 ass attribute
contains a specific value. 
The method has one parameter: the class name which is given in quotes within the parentheses
after the method name. 
Because several elements can have the same value for their cl ass attribute, this method
always returns a Nodelist.

# SELECTING ELEMENTS USING CSS SELECTORS 
querySe 1 ector() returns the first element node that matches the CSS-style selector.
querySe 1ectorA11 () returns a Nodelist of all of the matches.
Both methods take a CSS selector as their only parameter.
The CSS selector syntax offers more flexibility and accuracy when selecting an element than
just specifying a class name or a tag name, and should also be familiar to front-end web
developers who are used to targeting elements using CSS.

LOOPING THROUGH A NODELIST
If you want to apply the same code to numerous elements, looping through a Nodelist is a
powerful technique. 
It involves finding out how many items are in the Nodelist, and then setting a counter to loop
through them, one-by-one.
Each time the loop runs, the script checks that the counter is less than the total number of
items in the Nodelist.

# TRAVERSING THE DOM 
When you have an element node, you can selec another element in relation to it using these five
properties. This is known as traversing the DOM. 
# parentNode
This property finds the element node for the containing (or parent) element in the HTML.
(1) If you started with the first <l i >element, then its parent node would be the one
representing the <ul >element.

# previousSibling nextSibling
These properties find the previous or next sibling of a node if there are siblings.
If you started with the first <1 i > element, it would not have a previous sibling. However, its next
sibling (2) would be the node representing the second <l i >.

# firstChil d lastChild
These properties find the first or last child of the current element.
If you started with the <u 1 > element, the first child would be the node representing the first
<l i> element, and (3) the last child would be the last <1 i >.


# WHITESPACE NODES 
Traversing the DOM can be difficult because some browsers add a text node whenever they
come across whitespace between elements.
Most browsers, except IE, treat whitespace between elements (such as spaces or carriage
returns) as a text node, so the properties below return different elements in different browsers: 
Below, you can see all of the whitespace nodes added to the  DOM tree for the list example.
Each one is represented by a green square. You could strip all the whitespace out of a page
before serving it to the browser. This would also make the page smaller and faster to serve/load.
However, it would also make the code much harder to read.

# PREVIOUS & NEXT SIBLING
You have just seen that these properties can return inconsistent results in different browsers. However, it is safe to use them when there is no whitespace between elements.

# FlRST & LAST CHILD
These properties also return inconsistent results if there is whitespace between elements.
In this example, a slightly different solution is used in the HTML - the closing tags are put 
next to the opening tags of the next element, making it a little more readable. The
example starts by using the getElementsByTagName() method to select the <ul> 

# HOW TO GET/UPDATE ELEMENT CONTENT
So far this chapter has focused on finding elements in the DOM tree. The rest of this chapter shows how to access/update element content. Your choice of techniques depends upon what the element contains. 
