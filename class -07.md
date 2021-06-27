# HTML5: Figure and Figure Caption
# <figure>
Images often come with captions. HTML5 has introduced a new <figure> element to
contain images and their caption so that the two are associated.
You can have more than one image inside the <figure> element as long as they all share
the same caption.

# <figcaption>
The <figcaption> element has been added to HTML5 in order to allow web page authors to add
a caption to an image. Before these elements were created there was no way to
associate an <img> element with its caption.


# Summary IMAGES
1- The <img> element is used to add images to a web page.
2- You must always specify a src attribute to indicate the source of an image and an alt attribute to describe the content of an image.
3- You should save images at the size you will be using them on the web page and in the appropriate format.
4- Photographs are best saved as JPEGs; illustrations or logos that use flat colors are better saved as GIFs.

# Tables
1- How to create tables
2- What information suits tables
3- How to represent complex data in tables



There are several types of information that need to be displayed in a grid or table. For example: sports results, stock reports, train timetables.
When representing information in a table, you need to think in terms of a grid made up of rows and columns (a bit like a spreadsheet). In this chapter you will learn how to:
● Use the four key elements for creating tables
● Represent complex data using tables
● Add captions to tables


# What's a Table?
A table represents information in a grid format.
Examples of tables include financial reports, TV schedules, and sports results.


# Basic Table Structure
<table>
The <table> element is used to create a table. The contents of the table are written out row by row.
<tr>
You indicate the start of each row using the opening <tr> tag. (The tr stands for table row.)
It is followed by one or more<td> elements (one for each cell x in that row).At the end of the row you use a
closing </tr> tag.
<td>
Each cell of a table is represented using a <td>element. (The td stands for table data.)

# Table Headings
<th>
The <th> element is used just like the <td> element but its purpose is to represent the
heading for either a column or a row. (The th stands for table heading.)
Even if a cell has no content, you should still use a <td> or <th> element to represent
the presence of an empty cell otherwise the table will not render correctly. (The first cell
in the first row of this example shows an empty cell.)
Using <th> elements for headings helps people who use screen readers, improves
the ability for search engines to index your pages, and also enables you to control the
appearance of tables better when you start to use CSS


# Spanning ColumnS
Sometimes you may need the entries in a table to stretch across more than one column.
The colspan attribute can be used on a <th> or <td> element and indicates how many columns
that cell should run across. In the example on the right you can see a timetable with
five columns; the first column contains the heading for that row (the day), the remaining four
represent one hour time slots

# Spanning Rows
ou may also need entries in a table to stretch down across more than one row.
The rowspan attribute can be used on a <th> or <td> element to indicate how many rows a cell
should span down the table. In the example on the left you can see that ABC is showing a
movie from 6pm - 8pm, whereas the BBC and CNN channels are both showing two programs
during this time period (each of which lasts one hour).

# Long Tables
There are three elements that help distinguish between the main content of the table and
the first and last rows (which can contain different content). These elements help people
who use screen readers and also allow you to style these sections in a different manner than the
rest of the table (as you will see when you learn about CSS).

<thead>
The headings of the table should sit inside the <thead> element. 
<tbody>
The body should sit inside the <tbody> element.
<tfoot>
The footer belongs inside the <tfoot> element. By default, browsers rarely treat
the content of these elements any differently than other elements however designers
often use CSS styles to change their appearance.

# Old Code:
# Width & Spacing
e are some outdated attributes which you should not use on new websites. You may,
however, come across some of them when looking at older code, so I will mention them
here. All of these attributes have been replaced by the use of CSS.
The width attribute was used on the opening <table> tag to indicate how wide that table
should be and on some opening <th> and <td> tags to specify the width of individual cells.
The value of this attribute is the width of the table or cell in pixels.

# Border & Background
The border attribute was used on both the <table> and <td> elements to indicate the width of
the border in pixels. The bgcolor attribute was used to indicate background colors
of either the entire table or individual table cells




# JS

# HOW MEMORY & VARIABLES WORK 
Global variables use more memory. The browser has to remember them for as long as the web page using them is loaded. Local variables are only remembered during the period of time that a function is being executed. 

# CREATING THE VARIABLES IN CODE
Each variable that you declare takes up memory. The more variables a browser has to remember,
the more memory your script requires to run. Scripts that require a lot of memory can perform
slower, which in turn makes your web page take longer to respond to the user

# NAMING COLLISIONS
You might think you would avoid naming collisions; after all you know which variables you are using.
But many sites use scripts written by several people. If an HTML page uses two JavaScript files, and both
have a global variable with the same name, it can cause errors. Imagine a page using these two scripts:

# CREATING MORE OBJECT LITERALS
Here you can see another object. Again it is called hote 1, but this
time the model represents a different hotel. For a moment, imagine that this is a different
page of the same travel website. The Park hotel is larger. It has 120 rooms and 77 of them are
booked. 
The only things changing in the code are the values of the hot e 1 object's properties:
• The name of the hotel
• How many rooms it has
• How many rooms are booked 

# CREATING OBJECTS USING CONSTRUCTOR SYNTAX 
On the right, an empty object called hote 1 is created using the constructor function.
Once it has been created, three properties and a method are
then assigned to the object. (If the object already had any of these properties, this would
overwrite the values in those properties.)
To access a property of this object, you can use dot notation, just as you can with any object.

# ADDING AND REMOVING PROPERTIES
Once you have created an object (using literal or constructor notation), you can add new
properties to it.
You do this using the dot notation that you saw for adding properties to objects on pl03.
In this example, you can see that an instance of the hotel object
is created using an object literal. Immediately after this, the
hotel object is given two extra properties that show the facilities (whether or not it has
a gym and/or a pool). These properties are given values that are Booleans (true or false).

# RECAP: STORING DATA
n JavaScript, data is represented using name/value pairs.
To organize your data, you can use an array or object to group a set of related values. In arrays and objects the name is also known as a key.

# VARIABLES
A variable has just one key (the variable name) and one value. 

# ARRAYS
Arrays can store multiple pieces of information. Each piece of information is separated by a comma.
The order of the values is important because items in an array are assigned a number (called an index).

# INDIVIDUAL OBJECTS
Objects store sets of name/value pairs. They can be properties (variables) or methods (functions).
The order of them is not important (unlike the array). You access each piece of data by its key. 

# MULTIPLE OBJECTS
When you need to create multiple objects within the same page, you should use an object constructor to
provide a template for the objects.


# WHAT ARE BUILT-IN OBJECTS?
Browsers come with a set of built-in objects that represent things like the browser window and the current web page shown in that window. These built-in objects act like a toolkit for creating interactive web pages.
The objects you create will usually be specifically written to suit your needs. They model the data
used within, or contain functionality needed by, your script. Whereas, the built-in objects contain
functionality commonly needed by many scripts. As soon as a web page has loaded into the browser,
these objects are available to use in your scripts. 

# USING THE BROWSER OBJECT MODEL
Here, data about the browser is collected from the window object and its children, stored in the msg
variable, and shown in the page. The+= operator adds data onto the end of the msg variable.

1. Two of the window object's properties, i nnerWi dth and i nnerHei ght, show width and
height of the browser window
2. Child objects are stored as properties of t heir parent object. So dot notation is used to access
them, just like you would access any other property of that object.

3. The element whose id attribute has a value of info is selected, and the message that
has been built up to this point is written into the page. 

# USING THE DOCUMENT OBJECT
This example gets information about the page, and then adds that information to the footer.
1. The details about the page are collected from properties of the document object.
JAVASCRIPT
These details are stored inside a variable called msg, along with HTML markup to display
the information. Again, the += operator adds the new value onto the existing content of the
msg variable.
2. You have seen the document object's get El ementByid () method in several examples so
far. It selects an element from the page using the value of its id attribute. You will see this
method in more depth on p195