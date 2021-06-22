# Definition Lists

<dl>
The definition list is created with the <dl> element and usually consists of a series of terms and
their definitions. Inside the <dl> element you will usually see pairs of <dt> and <dd> elements.

<dt>
This is used to contain the term being defined (the definition term).

<dd>
This is used to contain the definition.

# Nested Lists
You can put a second list inside an <li> element to create a sublist or nested list.

# Summary LISTS
1- There are three types of HTML lists: ordered, unordered, and definition.
2- Ordered lists use numbers.
3- Unordered lists use bullets.
4- Definition lists are used to define terminology.
5- Lists can be nested inside one another.

# Link
-[x] Creating links between pages
-[x] Linking to other sites
-[x] Email links

# Links are the defining feature of the web because they allow you to move from one web page to another — enabling the very idea of browsing or surfing.

You will commonly come across the following types of links:
● Links from one website to another
● Links from one page to another on the same website
● Links from one part of a web page to another part of the
same page
● Links that open in a new browser window
● Links that start up your email program and address a new
email to someone


# Linking to Other Sites
<a> 
chapter-04/linking-to-other-sites.html HTML Links are created using the <a> element which has an attribute
called href. The value of the href attribute is the page that you want people to go to when they click 
on the link.
Users can click on anything that appears between the opening <a> tag and the closing </a> tag and will be taken to the page specified in the href attribute.
When you link to a different website, the value of the href attribute will be the full web
address for the site, which is known as an absolute URL.


# Linking to Other Pages on the Same Site
<a>
When you are linking to other pages within the same site, you do not need to specify the
domain name in the URL. You can use a shorthand known as arelative URL.
If all the pages of the site are in the same folder, then the value of the href attribute is just the
name of the file.
If you have different pages of a site in different folders, then you can use a slightly more complex
syntax to indicate where the page is in relation to the current page. You will learn more about
these on the pages 81-84.
If you look at the download code for each chapter, you will see that the index.html file contains links that use relative URLs.

# Relative URLs
When you are linking to a page on your own website, you do not need to specify the domain name. You can use relative URLs which are a shorthand way to tell the browser where a page is in relation to the current page.
This is especially helpful when creating a new website or learning about HTML because you can create links between pages when they are only on your personal computer(before you have got a domain name and uploaded them to the web).
Because you do not need to repeat the domain name in each link, they are also quicker to write.

# Email Links
# Milto
To create a link that starts up the user's email program and addresses an email to a specified
email address, you use the <a> element. However, this time the value of the href attribute starts
with mailto: and is followed by the email address you want the email to be sent to.
On the right you can see that an email link looks just like any other link but, when it is clicked
on, the user's email program will open a new email message and address it to the person specified in the link.


# Opening Links in a New Window
# Target
If you want a link to open in a new window, you can use the target attribute on the opening
<a> tag. The value of this attribute should be _blank.
One of the most common reasons a web page author might want a link to be opened in a new window is if it points to another website. In such cases,
they hope the user will return to the window containing their site after finishing looking at the other one.

# Linking to a Specific Part of the Same Page
At the top of a long page you might want to add a list of contents that links to the corresponding sections lower down. Or you might want to add a link from part way down the page back to the top of it to save
users from having to scroll back to the top.
Before you can link to a specific part of a page, you need to identify the points in the page
that the link will go to. You do this using the id attribute (which can be used on every HTML
element). You can see that the <h1> and <h2> elements in this example have been given id
attributes that identify those sections of the page.
The value of the id attribute should start with a letter or an underscore (not a number or
any other character) and, on a single page, no two id attributes should have the same value.



# Summary LISTS, TABLES AND FORMS
- In addition to the CSS properties covered in other chapters which work with the contents of all elements,
there are several others that are specifically used to control the appearance of lists, tables, and forms.

- List markers can be given different appearances using the list-style-type and list-style image properties.

- Table cells can have different borders and spacing in different browsers, but there are properties you can
use to control them and make them more consistent.

- Forms are easier to use if the form controls are vertically aligned using CSS.

- Forms benefit from styles that make them feel more interactive.

# Layout
1- Controlling the position of elements
2- Creating site layouts
3- Designing for different sized screens



# In this chapter we are going to look at how to control where each element sits on a page and how to create attractive page layouts.

This involves learning about how designing for a screen can be
different to designing for other mediums (such as print). In this
chapter we will:
● Explore different ways to position elements using normal flow, relative positioning, absolute positioning and floats.
● Discover how various devices have different screen sizes and resolution, and how this affects the design process.
● Learn the difference between fixed width and liquid layouts, and how they are created.
● Find out how designers use grids to make their page designs look more professional.


# Key Concepts in Positioning Elements
**Building Blocks CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box.**
Block-level boxes start on a new line and act as the main building blocks of any layout, while inline boxes flow between surrounding text. You can control how much space each box takes up by setting the width of the
boxes (and sometimes the height, too). To separate boxes, you can use borders, margins, padding, and background colors. 

**Block-level elements**
start on a new line Examples include:
<h1> <p> <ul> <li>


**flow in between**
surrounding text Examples include:
<img> <b> <i>


# Containing Elements
If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element.
It is common to group a number of elements together inside a <div> (or other block-level) element. For example, you might group together all of the elements that form the header of a site (such as the logo and
the main navigation). The <div> element that contains this group of elements is then referred to as the containing element.


# Controlling the Position of Elements
CSS has the following positioning schemes that allow you to control the layout of a page: normal flow, relative positioning, and absolute positioning. You specify the positioning scheme using the position
property in CSS. You can also float elements using the float property.


# Normal flow
Every block-level element appears on a new line, causing each item to appear lower down
the page than the previous one.
Even if you specify the width of the boxes and there is space for two elements to sit side-byside, they will not appear next to each other. This is the default behavior (unless you tell the browser to do something else)


# Relative Positioning
This moves an element from the position it would be in normal flow, shifting it to the top, right,
bottom, or left of where it would have been placed. This does not affect the position of surrounding 
elements; they stay in the position they would be in in normal flow

# Absolute positioning
This positions the element in relation to its containing element. It is taken out of normal flow,
 meaning that it does not affect the position of any surrounding elements (as they simply ignore the
space it would have taken up).
Absolutely positioned elements move as users scroll up and down the page.


To indicate where a box should be positioned, you may also need to use box offset properties to tell the browser how far from the top or bottom and left or right it should be placed. (You will meet these when we
introduce the positioning schemes on the following pages.)

When you move any element from normal flow, boxes can overlap. The z-index propert allows you to control
which box appears on top.

# Normal Flow
**position:static**
In normal flow, each block-level element sits on top of the next one. Since this is the default
way in which browsers treat HTML elements, you do not need a CSS property to indicate
that elements should appear in normal flow, but the syntax would be:
**position: static;**
I have not specified a width property for the heading element, so you can see how it stretches the 
width of the entire browser window by default.
The paragraphs are restricted to 450 pixels wide. This shows how the elements in normal flow
start on a new line even if they do not take up the full width of the browser window.

# position:relative
Relative positioning moves an element in relation to where it would have been in normal flow.
For example, you can move it 10 pixels lower than it would have been in normal flow or 20% to
the right.
You can indicate that an element should be relatively positioned using the position property
with a value of relative.
You then use the offset properties (top or bottom and left or right) to indicate how far to move the element from where it would have been in normal flow.
To move the box up or down, you can use either the top or bottom properties.

# position:absolute
When the position property is given a value of absolute, the box is taken out of normal
flow and no longer affects the position of other elements on the page. (They act like it is not
there.)
The box offset properties (top or bottom and left or right) specify where the element
should appear in relation to its containing element.
In this example, the heading has been positioned at the top of the page and 500 pixels from its left
edge. The width of the heading is set to be 250 pixels wide.
The width property has also been applied to the <p> elements in this example
to prevent the text from overlapping and becoming unreadable.

# position:fixed
Fixed positioning is a type of absolute positioning that requires the position property
to have a value of fixed.
It positions the element in relation to the browser window.
Therefore, when a user scrolls down the page, it stays in the exact same place. It is a good
idea to try this example in your browser to see the effect.
To control where the fixed position box appears in relation to the browser window, the box
offset properties are used.
In this example, the heading has been positioned to the top left hand corner of the browser
window. When the user scrolls down the page, the paragraphs disappear behind the heading.
The <p> elements are in normal flow and ignore the space that the <h1> element would have
taken up. Therefore, the margin-top property has been used to push the first <p>
element below where the fixed position <h1> element is sitting.

# z-index
When you use relative, fixed, or absolute positioning, boxes can overlap. If boxes do overlap, the
elements that appear later in the HTML code sit on top of those that are earlier in the page.
If you want to control which element sits on top, you can use the z-index property. Its value
is a number, and the higher the number the closer that element is to the front. For example, an
element with a z-index of 10 will appear over the top of one with a z-index of 5.


# float
The float property allows you to take an element in normal flow and place it as far to the
left or right of the containing element as possible.
Anything else that sits inside the containing element will flow around the element that is floated.
When you use the float property, you should also use the width property to indicate how
wide the floated element should be. If you do not, results can be inconsistent but the box is likely
to take up the full width of the containing element (just like it would in normal flow).

# Using Float to Place Elements Side-by-Side
A lot of layouts place boxes next to each other. The float property is commonly used to
achieve this.
When elements are floated, the height of the boxes can affect where the following elements sit.
In this example, you can see six paragraphs, each of which has a width and a float property set.
The fourth paragraph does not go across to the left hand edge of the page as one might expect.
Rather it sits right under the third paragraph.
The reason for this is that the fourth paragraph has space to start under the third paragraph,
but it cannot go any further to the left because the second paragraph is in the way.

# Clear
The clear property allows you to say that no element (within the same containing element)
should touch the left or righthand sides of a box. It can take the following values:

# left
The left-hand side of the box should not touch any other elements appearing in the same
containing element.

# right
The right-hand side of the box will not touch elements appearing in the same containing
element.

# both
Neither the left nor right-hand sides of the box will touch elements appearing in the same
containing element.

# none
Elements can touch either side. In this example, the fourth paragraph has a class called
clear. The CSS rule for this class uses the clear property to indicate that nothing should
touch the left-hand side of it. The fourth paragraph is therefore moved further down the page
so no other element touches its left-hand side.

# width
This sets the width of the columns.

# float
This positions the columns next to each other.

# margin
This creates a gap between the columns.
A two-column layout like the one shown on this page would need two <div> elements, one for the
main content of the page and one for the sidebar.
Inside each of the <div> elements there can be headings, paragraphs, images, and even
other <div> elements.

# Bage Size
Because screen sizes and display resolutions vary so much, web designers often try to create pages of around 960-1000 pixels wide (since most users will be able to see designs this wide on their screens).

# Fixed Width Layouts
Fixed width layout designs do not change size as the user increases or decreases the size of 
their browser window.
Measurements tend to be given in pixels.


# A Fixed Width Layout
To create a fixed width layout, the width of the main boxes on a page will usually be specified
in pixels (and sometimes their height, too).
Here you can see several <div> elements, each of which uses an id or class attribute to indicate
its purpose on the page.
In a book like this, the result of both the fixed and liquid layouts look similar. To get a real feel for
them, you need to view them in your browser and see how they react when you adjust the size of
the browser window.
The fixed width layout will stay the same width no matter what size the browser window is,
whereas the liquid layout will stretch (or shrink) to fill the screen.


# A Liquid Layout
The liquid layout uses percentages to specify the width of each box so that the design will stretch
to fit the size of the screen.


# CSS Frameworks
CSS frameworks aim to make your life easier by providing the code for common tasks, such as creating layout grids, styling forms, creating printer-friendly versions of pages and so on. You can include the CSS
framework code in your projects rather than writing the CSS from scratch.

# ADVANTAGES
● They save you from repeatedly writing code for the same tasks.
● They will have been tested across different browser versions (which helps avoid browser bugs).


 # DISADVANTAGES
● They often require that you use class names in your HTML code that only control the presentation of the page
(rather than describe its content).

# A Grid-Based Layout Using 960.G
Let's take a look at an HTML page and how it has been marked up to use the 960.gs grid
system.
You can see that we include the CSS for the grid using the <link> element inside the
<head> of the page.
The styles we are writing ourselves are shown on the right hand page.
The 960_12_col.css stylesheet contains all of the rules we need to control the grid layout. The
HTML uses the class names: 
container_12 to act as a container for the whole page and indicate that we are using a 12
column grid clearfix to ensure that browsers know the height of the containing box, because it only
contains floated elements (this addresses the issue you met on pages 371-372)


# Multiple Style Sheets
# @import
Some web page authors split up their CSS style rules into separate style sheets. For
example, they might use one style sheet to control the layout and another to control fonts,
colors and so on.
Some authors take an even more modular approach to stylesheets, creating separate stylesheets to control
typography, layout, forms, tables, even different styles for each sub-section of a site.
There are two ways to add multiple style sheets to a page:


# link
On this page you can see the other technique for including multiple style sheets. Inside the
<head> element is a separate <link> element for each style sheet.
The contents of site.css are identical to styles.css on the left hand page, except the code
does not contain @import rules.
As with all style sheets, if two rules apply to the same element then rules that appear later in a
document will take precedence over previous rules. 
