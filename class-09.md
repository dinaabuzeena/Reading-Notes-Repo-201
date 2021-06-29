# Old Code: Width & Spacing
There are some outdated attributes which you should not use on new websites. You may,
however, come across some of them when looking at older code, so I will mention them
here. All of these attributes have been replaced by the use of CSS. The width attribute was used
on the opening <table> tag to indicate how wide that table should be and on some opening
<th> and <td> tags to specify the width of individual cells. The value of this attribute is
the width of the table or cell in pixels.

# Border & Background
The border attribute was used on both the <table> and <td> elements to indicate the width of
the border in pixels.
The bgcolor attribute was used to indicate background colors of either the entire table or
individual table cells


# Summary TABLES
X The <table> element is used to add tables to a web page.
X A table is drawn out row by row. Each row is created with the <tr> element.
X Inside each row there are a number of cells represented by the <td> element (or <th> if it is a
header).
X You can make cells of a table span more than one row or column using the rowspan and colspan attributes.
X For long tables you can split the table into a <thead>, <tbody>, and <tfoot>.

# Forms

X How to collect information from visitors
X Different kinds of form controls
X New HTML5 form controls


Traditionally, the term 'form' has referredto a printed document that contains
spaces for you to fill in information.
HTML borrows the concept of a form to refer to different elements that allow you to collect information from visitors to your site.
Whether you are adding a simple search box to your website or you need to create more complicated insurance applications, HTML forms give you a set of elements to collect data from your users. In this chapter you will learn:
● How to create a form on your website
● The different tools for collecting data
● New HTML5 form controls


# Form Structure

<form>
Form controls live inside a <form> element. This element should always carry the action
attribute and will usually have a method and id attribute too.
<action>
Every <form> element requires an action attribute. Its value is the URL for the page on the
server that will receive the information in the form when it is submitted.

<method>
Forms can be sent using one of two methods: get or post.

# Text Input
<input>
The <input> element is used to create several different form controls. The value of the type
attribute determines what kind of input they will be creating.
** type="text"**
When the type attribute has a value of text, it creates a singleline text input.
# name
When users enter information into a form, the server needs to know which form control each
piece of data was entered into.
(For example, in a login form, the server needs to know what has been entered as the username
and what has been given as the password.) Therefore, each form control requires a name attribute.
The value of this attribute identifies the form control and is sent along with the information
they enter to the server.

# Password Input

<input>
type="password"
When the type attribute has a value of password it creates a text box that acts just like a
single-line text input, except the characters are blocked out. They are hidden in this way so
that if someone is looking over the user's shoulder, they cannot see sensitive data such as passwords.
name
The name attribute indicates the name of the password input, which is sent to the server with
the password the user enters. size, maxlength It can also carry the size and
maxlength attributes like the the single-line text input.


# Text Are
<textarea>
The <textarea> element is used to create a mutli-line text input. Unlike other input
elements this is not an empty element. It should therefore have an opening and a closing tag.

Any text that appears between the opening <textarea> and closing </textarea> tags will
appear in the text box when the page loads.

If the user does not delete any text between these tags, this message will get sent to the
server along with whatever the user has typed. (Some sites use JavaScript to clear this
information when the user clicks in the text area.)


# Radio Button

<input>
type="radio"
Radio buttons allow users to pick just one of a number of options.
name
The name attribute is sent to the server with the value of the option the user selects. When
a question provides users with options for answers in the form of radio buttons, the value of
the name attribute should be the same for all of the radio buttons used to answer that question.
value
The value attribute indicates the value that is sent to the server for the selected option.
The value of each of the buttons in a group should be different (so that the server knows which
option the user has selected).
checked
The checked attribute can be used to indicate which value (if any) should be selected when
the page loads. The value of this attribute is checked. Only one radio button in a group should
use this attribute.


# Checkbox
<input>
type="checkbox"
Checkboxes allow users to select (and unselect) one or more options in answer to a question.
name
The name attribute is sent to the server with the value of the option(s) the user selects. When
a question provides users with options for answers in the form of checkboxes, the value of the name attribute should be the same for all of the buttons that answer that question.
value
The value attribute indicates the value sent to the server if this checkbox is checked.
checked
The checked attribute indicates that this box should be checked when the page loads. If used, its
value should be checked.


# Drop Down List Box

<select>
A drop down list box (also known as a select box) allows users to select one option from a
drop down list.
The <select> element is used to create a drop down list box. It contains two or more <option>
elements.
name
The name attribute indicates the name of the form control being sent to the server, along with the value the user selected.
<option>
The <option> element is used to specify the options that the user can select from. The words
between the opening <option>
and closing </option> tags will be shown to the user in the drop down box.


# Multiple Select Box
<select>
size
You can turn a drop down select box into a box that shows more than one option by adding the
size attribute. Its value should be the number of options you want to show at once. In the
example you can see that three of the four options are shown.
Unfortunately, the way that browsers have implemented this attribute is not perfect, and it
should be tested throroughly if used (in particular in Firefox and Safari on a Mac).
multiple You can allow users to select multiple options from this list by adding the multiple attribute
with a value of multiple.

# File Input Box
<input>
If you want to allow users to upload a file (for example an image, video, mp3, or a PDF),
you will need to use a file input 
box.
type="file" This type of input creates a box that looks like a text input
followed by a browse button.
When the user clicks on the browse button, a window opens up that allows them to select a
file from their computer to be uploaded to the website.

# Submit Button
input>
type="submit" The submit button is used to send a form to the server.
name
It can use a name attribute but it does not need to have one.
value
The value attribute is used to control the text that appears on a button. It is a good idea to
specify the words you want to appear on a button because the default value of buttons on some
browsers is ‘Submit query’ and this might not be appropriate for all kinds of form

 # image Button
input>
type="image"
If you want to use an image for the submit button, you can give the type attribute a value of
image. The src, width, height, and alt attributes work just like they do when used with the
<img> elemen

# Button & hidden Controls
<button>
The <button> element was introduced to allow users more control over how their buttons
appear, and to allow other elements to appear inside the button.
This means that you can combine text and images between the opening <button>
tag and closing </button> tag.
<input>
type="hidden" This example also shows a hidden form control. These form
controls are not shown on the page (although you can see them if you use the View Source option
in the browser). They allow web page authors to add values to forms that users cannot see.
For example, a web page author might use a hidden field to indicate which page the user was
on when they submitted a form.

# Labelling Form Controls
<label>
When introducing form controls, the code was kept simple by indicating the purpose of each
one in text next to it. However, each form control should have its own <label> element as this
makes the form accessible to vision-impaired users. The <label> element can be
used in two ways. It can: 1. Wrap around both the text description and the form input
(as shown on the first line of the example to your right). 2. Be kept separate from the
form control and use the for attribute to indicate which form control it is a label for (as shown
with the radio buttons).

# Grouping Form Elements
<fieldset>
You can group related form controls together inside the <fieldset> element. This is
particularly helpful for longer forms.
Most browsers will show the fieldset with a line around the edge to show how they are
related. The appearance of these lines can be adjusted using CSS.
<legend>
The <legend> element can come directly after the opening <fieldset> tag and contains a
caption which helps identify the purpose of that group of form controls.

# HTML5: Form Validation
You have probably seen forms on the web that give users messages if the form control has
not been filled in correctly; this is known as form validation. Traditionally, form validation
has been performed using JavaScript (which is beyond the scope of this book). But HTML5
is introducing validation and leaving the work to the browser.