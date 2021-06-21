# Chapter 3: Lists
**Author Details**

<address> 
chapter-02/address.html HTML The <address> element has quite a specific use: to contain
contact details for the author of the page. It can contain a physical address,but it does not have to. 
Forexample, it may also contain aphone number or email address.


**Changes to Content**
<ins>
<del>
The <ins> element can be used to show content that has been inserted into a document, while
the <del> element can show text that has been deleted from it.

<s>
The <s> element indicates something that is no longer accurate or relevant (but thatshould not be deleted).
Visually the content of an <s> element will usually be displayed with a line through the center.

# Summary TEXT
X HTML elements are used to describe the structure of the page (e.g. headings, subheadings, paragraphs).
X They also provide semantic information (e.g. where emphasis should be placed, the definition of any
acronyms used, when given text is a quotation).


# Lists
1- Ordered lists are lists where each item in the list is numbered. For example, the list might be a set of steps for a recipe that must be performed in order, or a legal contract where each point needs to be identified by a section number.
2- Unordered lists are lists that begin with a bullet point (rather than characters that indicate order).
3- Definition lists are made up of a set of terms along with the definitions for each of those terms.

# Ordered Lists
<ol>
The ordered list is created with the <ol> element.

<li>
Each item in the list is placed between an opening <li> tag and a closing </li> tag. 
(The listands for list item.)


# SummaryTEXT
-[x] There are properties to control the choice of font, size, weight, style, and spacing.
-[x] There is a limited choice of fonts that you can assume most people will have installed.
-[x] If you want to use a wider range of typefaces there are several options, but you need to have the right icense to use them.
-[x] You can control the space between lines of text, individual letters, and words. Text can also be aligned
to the left, right, center, or justified. It can also be indented.
-[x] You can use pseudo-classes to change the style of an element when a user hovers over or clicks on text, or
when they have visited a link.

# Boxes
*At the beginning of this section on CSS, you saw how CSS treats each HTML element as if it lives
 in its own box
You can set several properties that affect the appearance of these boxes. In this chapter you will see how to:
● Control the dimensions of your boxes
● Create borders around boxes
● Set margins and padding for boxes
● Show and hide boxes


# Box Dimention
**width, height**
By default a box is sized just big enough to hold its contents. To set your own dimensions for a box you can use the height and width properties.
The most popular ways to specify the size of a box are to use pixels, percentages, or ems. Traditionally, pixels have been the most popular method because they allow designers to accurately control their size.
When you use percentages, the size of the box is relative to the size of the browser window or, if the box is encased within another box, it is a percentage of the size of the containing box.
When you use ems, the size of the box is based on the size of text within it. Designers have recently started to use percentages and ems more for measurements as they try to create designs that are flexible across devices which have different-sized screens.

# Limiting Width
**min-width, max-width**
ome page designs expand and  shrink to fit the size of the user's screen. In such designs, the
min-width property specifies the smallest size a box can be displayed at when the browser window is narrow, and the max-width property indicates the maximum width a box can stretch to when the browser window is wide.
These are very helpful properties to ensure that the content of pages are legible (especially on the smaller screens of handheld devices). For example, you can use the max-width property to ensure that lines of text do not appear too wide within a big browser window and you can use the min-width property to make sure that they do not appear too narrow.
You may find it helpful to try this example out in your browser so that you can see what happens when you increase or decrease the size of the browser window

# Limiting Hight
**min-height, max-height**
In the same way that you might want to limit the width of a box on a page, you may also want to limit the height of it. This is achieved using the min-height and max-height properties.
The example on this page demonstrates these properties in action. It also shows you what happens when the content of the box takes up more space than the size specified for the box.
If the box is not big enough to hold the content, and the content expands outside the box it can
look very messy. To control what happens when there is not enough space for the content of
a box, you can use the overflow property, which is discussed on the next page.


# Overflowing Content
**over flow**
The overflow property tells the browser what to do if the content contained within a box is larger
than the box itself. It can have one of two values

 # hidden 
 This property simply hides any extra content that does not fit in the box.

# scroll
This property adds a scrollbar to the box so that users can scroll to see the missing content.
On the left, you can see two boxes whose contents expand beyond their set dimensions. The first example has the overflow property with a value of hidden.
The second example has the overflow property with a value of scroll.
The overflow property is particularly handy because some browsers allow users to adjust
the size of the text to appear as large or as small as they want. If the text is set too large then the
page can become an unreadable mess. Hiding the overflow on such boxes helps prevent items overlapping on the page.

# Border, Margin& Padding
1- Border
Every box has a border (even if it is not visible or is specified to be 0 pixels wide). The border separates the edge of one box from another

2- Margin
Margins sit outside the edge of the border. You can set the width of a margin to create a gap between the borders of two adjacent boxes.

3- Padding
Padding is the space between the border of a box and any content contained within it.
Adding padding can increase the readability of its contents.

# Border Width
**border-width**
The border-width property is used to control the width of a border. The value of this property can either be given in pixels or using one of the following values:
thin
medium
thick


# Border Style
You can control the style of a border using the border-style property. This property can take
the following values:

**solid** 
a single solid line 

# dotted 
a series of square dots (if your border is 2px wide, then the dots are 2px squared with a 2px gap between each dot) 

# dashed 
a series of short lines 

# double
 two solid lines (the value of the border-width property creates the sum of the two lines) 

# groove
 appears to be carved
into the page

# ridge 
appears to stick out from the page

# inset
 appears embedded into the page

# outset 
looks like it is coming out of the screen

# hidden
 none no border is shown You can individually change the styles of different borders using:
border-top-style
border-left-style
border-right-style
border-bottom-style

# Border Color
You can specify the color of a border using either RGB values, hex codes or CSS color names
(as you saw on pages 251-252).

It is possible to individually control the colors of the borders on different sides of a box using:
border-top-color border-right-color border-bottom-color border-left-color It is also possible to use a
shorthand to control all four border colors in the one property:
border-color: darkcyan deeppink darkcyan deeppink; The values here appear in clockwise order: top, right,
bottom, left.

# Shorthand
**border**
The border property allows you to specify the width, style and color of a border in one property (and the values should be coded in that specific order)

# pandding
The padding property allows you to specify how much space should appear between the content of an element and its border.
The value of this property is most often specified in pixels (although it is also possible to use percentages or ems). If a percentage is used, the padding is a percentage of the browser window (or of the containing box
if it is inside another box).
Please note: If a width is specified for a box, padding is added onto the width of the box.
As you can see, the second paragraph here is much easier to read because there is a space between the text and the border of the box. 
The box is also wider because it has padding.
You can specify different values for each side of a box using:
padding-top
padding-right
padding-bottom
padding-left

# margin
 The margin property controls the gap between boxes. Its value is commonly given in pixels,
although you may also use percentages or ems.
If one box sits on top of another, margins are collapsed , which means the larger of the two
margins will be used and the smaller will be disregarded.
Please note: If the width of a box is specified then the margin is added to the width of the box.
You can specify values for each side of a box using:
margin-top
margin-right
margin-bottom
margin-left

# Change Inline/Block
**diplay**
The display property allows you to turn an inline element into a block-level element or vice
versa, and can also be used to hide an element from the page.
The values this property can take are:

# inline
This causes a block-level element to act like an inline element.

# block
This causes an inline element to act like a block-level element.

# inline-block
This causes a block-level element to flow like an inline element, while retaining other features of a block-level element.


# none
This hides an element from the page. In this case, the element acts as though it is not on the
page at all (although a user could still see the content of the box if
they used the view source option in their browser).
If you use this property, it is important to note that inline boxes are not supposed to create
block-level elements.

# Hiding Boxes
**visibity**
The visibility property allows you to hide boxes from users but It leaves a space where the
element would have been. This property can take two values:

# hidden
This hides the element.

# visible
This shows the element If the visibility of an element is set to hidden, a blank space will appear in its place.
If you do not want a blank space to appear, then you should use the display property with a value of none instead (as covered on the previous page).

