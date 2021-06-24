# Linking to a Specific Part of the Same Page
At the top of a long page you might want to add a list of contents that links to the
corresponding sections lower down. Or you might want to add a link from part way down the
page back to the top of it to save users from having to scroll back to the top.
Before you can link to a specific part of a page, you need to identify the points in the page
that the link will go to. You do this using the id attribute (which can be used on every HTML
element). You can see that the <h1> and <h2> elements in this example have been given id
attributes that identify those sections of the page

# nking to a Specific Part of Another Page
If you want to link to a specific part of a different page (whether on your own site or a different
website) you can use a similar technique.
As long as the page you are linking to has id attributes that identify specific parts of the
page, you can simply add the same syntax to the end of the link for that page.
Therefore, the href attribute will contain the address for the page (either an absolute URL or
a relative URL), followed by the # symbol, followed by the value of the id attribute that is used on
the element you are linking to.

# Summary LINKS
- Links are created using the <a> element.
- The <a> element uses the href attribute to indicate the page you are linking to.
-  If you are linking to a page within your own site, it is best to use relative links rather than qualified URLs.
- You can create links to open email programs with an email address in the "to" field.
- You can use the id attribute to target elements within a page that can be linked to.


# image 
1- How to add images to pages
2- Choosing the right format
3- Optimizing images for the web


There are several things to consider when selecting and preparing images for your site, but taking time to get them right will make it look more attractive and professional.
In this chapter you will learn how to:
● Include an image in your web pages using HTML
● Pick which image format to use
● Show an image at the right size
● Optimize an image for use on the web to make pages
load faste

# Choosing Images for Your Site
Images can be used to set the tone for a site in less time than it takes to read a description. If
you do not have photographs to use on your website, there are companies who sell stock
images; these are images you pay to use (there is a list of stock photography websites below).
Remember that all images are subject to copyright, and you can get in trouble for simply
taking photographs from another website.
If you have a page that shows several images (such as product photographs or members of a
team) then putting them on a simple, consistent background helps them look better as a group.



# Storing Images on Your Site
As a website grows, keeping images in a separate folder helps you understand how the
site is organized. Here you can see an example of the files for a website; all of the images are
stored in a folder called images.
On a big site you might like to add subfolders inside the images folder. For example, images such
as logos and buttons might sit in a folder called interface, product photographs might sit in a page
called products, and images related to news might live in a folder called news.
If you are using a content management system or blogging platform, there are usually tools
built into the admin site that allow you to upload images, and the program will probably
already have a separate folder for image files and any other uploads.


# Adding Images
<img> 
To add an image into the page you need to use an <img> element. This is an empty
element (which means there is no closing tag). It must carry the following two attributes:

# src
This tells the browser where it can find the image file. This will usually be a relative URL
pointing to an image on your own site. (Here you can see that the images are in a child folder
called images — relative URLs were covered on pages 83-84).

# alt
This provides a text description of the image which describes the image if you cannot see it.

# title
You can also use the title attribute with the <img> element to provide additional information
about the image. Most browsers will display the content of this attribute in a tootip when the
user hovers over the image.

# Height & Width  of Images
You will also often see an <img> element use two other attributes that specify its size:

# height
This specifies the height of the image in pixels.

# width
This specifies the width of the image in pixels. Images often take longer to load than the HTML code that
makes up the rest of the page.
It is, therefore, a good idea to specify the size of the image so that the browser can render
the rest of the text on the page while leaving the right amount of space for the image that is still
loading.

# Where to Place Images in Your Code
Where an image is placed in the code will affect how it is displayed. Here are three
examples of image placement that produce different results:
1: before a paragraph The paragraph starts on a new line after the image.
2: inside the start of a paragraph The first row of text aligns with the bottom of the image.
3: in the middle of a paragraph The image is placed between the words of the paragraph that it
appears in.

# Old Code: Aligning Images Horizontally
# align 
chapter-05/aligning-images-horizontally.html HTML The align attribute was
commonly used to indicate how the other parts of a page should flow around an image. It has
been removed from HTML5 and new websites should use CSS to control the alignment of images

# left
This aligns the image to the left (allowing text to flow around its right-hand side).

# right
This aligns the image to the right (allowing text to flow around its left-hand side).

# Old Code: Aligning Images Vertically
As you saw on the last page, the align attribute is no longer used in HTML5, but it is covered here
because you may see it used in older websites and it is still used in the code created by some
visual editors.

# top
This aligns the first line of the surrounding text with the top of the image.
# middle
This aligns the first line of the surrounding text with the middle of the image.

# bottom
This aligns the first line of the surrounding text with the bottom of the image.

# Three Rules for Creating Images
# 1 Save images in the right format
Websites mainly use images in jpeg, gif, or png format. If you choose the wrong image
format then your image might not look as sharp as it should and can make the web page
slower to load.

# 2 Save images at the right size
You should save the image at the same width and height it will appear on the website. If
the image is smaller than the width or height that you have specified, the image can be
distorted and stretched. If the image is larger than the width and height if you have specified,
the image will take longer to display on the page.

# 3 Use the correct resolution
Computer screens are made up of dots known as pixels. Images used on the web are also made
up of tiny dots. Resolution refers to the number of dots per inch, and most computer screens only
show web pages at 72 pixels per inch. So saving images at a higher resolution results in
images that are larger than necessary and take longer to download

# Tools to Edit & Save Images
The most popular tool amongst web professionals is Adobe Photoshop. (In fact, professional web designers often use this software to design entire sites.)
The full version of Photoshop is expensive, but there is a cheaper version called Photoshop
Elements which would suit the needs of most beginners.

# Image Dimensions
1- REDUCING IMAGE SIZE
You can reduce the size of images to create a smaller version of the image.

2- INCREASING IMAGE SIZE
You can't increase the size of photos significantly without affecting the image quality

3- CHANGING SHAPE
Only some images can be cropped without losing valuable information (see next page).

# Cropping Images
When cropping images it is important not to lose valuable information. It is best to source images that are the correct shape if possible.

# Image Resolution
JPGs, GIFs, and PNGs belong to a type of image format known as bitmap. They are made up of
lots of miniature squares. The resolution of an image is the number of squares that fit within
a 1 inch x 1 inch square area.
Images appearing on computer screens are made of tiny squares called pixels. A small segment
of this photograph has been magnified to show how it is made up of pixels. The web
browsers on most desktop computers display images at a resolution of 72 pixels per inch
(ppi). Images in print materials (such as books and magazines) are made up of tiny circles called
dots. These images are usually printed at a resolution of 300 dots per inch (dpi)

# Vector Images
When an image is a line drawing (such as a logo, illustration, or diagram), designers will often
create it in vector format. Vector formatted images are very different to bitmap images.
Vector images are created by placing points on a grid, and drawing lines between those
points. A color can then be added to "fill in" the lines that have been created.
The advantage of creating line drawings in vector format is that you can increase the dimensions
of the image without affecting the quality of it.

# Animated GIFs
Below you can see the individual frames that make up an animated GIF that shows an
orange dot revolving around a circle — like the kind of animation you might see when a
web page is loading.
Some image editing applications such as Adobe Photoshop allow you to create animated GIFs.
There are several tutorials about how to do this on the web. There are also several websites that
allow you to upload the graphics for the individual frames and create the animated GIF for you.
It is important to remember:
Each extra frame of the image increases the size of the file, and can therefore add to the time it
takes for an image to download (and web users do not like waiting a long time for images to
download).
Because GIFs are not an ideal format for displaying photographs, animated GIFs are really only suitable for simple illustrations.

# Transparenc
# Transparent GIF
If the transparent part of the image has straight edges and t is 100% transparent (that is,
not semi-opaque), you can save the image as a GIF (with the transparency option selected).

# PNG
If the transparent part of the image has diagonal or rounded edges or if you want a semiopaque transparency or a dropshadow, then you will need to save it as a PNG.



# How Css Rules Cascade
If there are two or more rules that apply to the same element, it is important to understand
which will take precedence.
# LAST RULE
If the two selectors are identical, the latter of the two will take precedence. Here you can see
the second i selector takes precedence over the first.
# SPECIFICITY
If one selector is more specific than the others, the more specific rule will take precedence
over more general ones. In this 
example:
h1 is more specific than * p b is more specific than p p#intro is more specific than p
# IMPORTANT
You can add !important after any property value to indicate that it should be considered
more important than other rules that apply to the same element.

# Inheritance
If you specify the font-family or color properties on the <body> element, they will apply
to most child elements. This is because the value of the font-family property is
inherited by child elements. It saves you from having to apply these properties to as many
elements (and results in simpler style sheets).
You can compare this with the background-color or border properties; they are not inherited by child elements. If these were inherited by all child elements then the page could look quite messy.

# Why use External Style Sheets?
All of your web pages can share the same style sheet. This is achieved by using the <link>
element on each HTML page of your site to link to the same CSS document. This means that the
same code does not need to be repeated in every page (which results in less code and smaller
HTML pages).
Therefore, once the user has downloaded the CSS stylesheet, the rest of the site will load
faster. If you want to make a change to how your site appears, you only need to edit the one
CSS file and all of your pages will be updated. For example, you can change the style of
every <h1> element by altering 

# Different versions of CSS & Browser Quirks
In the same way that there have been several versions of HTML, there have also been different
versions of CSS.
Browsers did not implement all CSS features at once, so some older browsers do not support
every property.
This is mentioned when it is likely to affect you, along with notes where CSS properties
might not behave as expected.

# Summary INTRODUCING CSS
1- CSS treats each HTML element as if it appears inside its own box and uses rules to indicate how that
element should look.
2- Rules are made up of selectors (that specify the elements the rule applies to) and declarations (that
indicate what these elements should look like).
3- Different types of selectors allow you to target your rules at different elements.
4- Declarations are made up of two parts: the properties of the element that you want to change, and the values
of those properties. For example, the font-family property sets the choice of font, and the value arial
specifies Arial as the preferred typeface.
5- CSS rules usually appear in a separate document, although they may appear within an HTML page.

# Color
1- How to specify colors
2- Color terminology and contrast
3- Background color

# Foreground Color
# color
The color property allows you to specify the color of text inside an element. You can specify any
color in CSS in one of three ways:
# rgb values
These express colors in terms of how much red, green and blue are used to make it up. For
example: rgb(100,100,90)
 # hex codes
These are six-digit codes that represent the amount of red, green and blue in a color,
preceded by a pound or hash # sign. For example: #ee3e80
# color names
There are 147 predefined color names that are recognized
by browsers. For example:
DarkCyan We look at these three different ways of specifying colors on the next double-page spread.
# background-color
CSS treats each HTML element as if it appears in a box, and the background-color property
sets the color of the background for that box.
You can specify your choice of background color in the same three ways you can specify
foreground colors: RGB values, hex codes, and color names (covered on the next page).
If you do not specify a background color, then the background is transparent.
By default, most browser windows have a white background, but browser users can set a background color for
their windows, so if you want to be sure that the background is white you can use the
background-color property on the <body> element.

# RGB Values
Values for red, green, and blue are expressed as numbers between 0 and 255.
# Hex Codes
Hex values represent values or red, green, and blue in hexadecimal code.
# Color Names
Colors are represented by predefined names. However, they are very limited in number.


# Contrast
ext is harder to read when there is low contrast between background and foreground
colors.
A lack of contrast is particularly a problem for those with visual impairments and color
blindness.
It also affects those with poor monitors and sunlight on their screens (which is increasingly
common as people use handheld devices outdoors).

# opacity, rgba
CSS3 introduces the opacity property which allows you to specify the opacity of an element
and any of its child elements.
The value is a number between 0.0 and 1.0 (so a value of 0.5 is 50% opacity and 0.15 is 15%
opacity).
The CSS3 rgba property allows you to specify a color, just like you would with an RGB value,
but adds a fourth value to indicate opacity. This value is known as an alpha value and is
a number between 0.0 and 1.0 (so a value of 0.5 is 50% opacity and 0.15 is 15% opacity). The
rgba value will only affect the element on which it is applied (not child elements).

# CSS3: HSL Colors
# hue
Hue is the colloquial idea of color. In HSL colors, hue is often represented as a color circle
where the angle represents the color, although it may also be shown as a slider with values
from 0 to 360.
# saturation
Saturation is the amount of gray in a color. Saturation is represented as a percentage.
100% is full saturation and 0% is a shade of gray.
# lightness
Lightness is the amount of white (lightness) or black (darkness) in a color. Lightness
is represented as a percentage.
0% lightness is black, 100% lightness is white, and 50% lightness is normal. Lightness
is sometimes referred to as luminosity.

# CSS3: HSL & HSLA
The hsl color property has been introduced in CSS3 as an alternative way to specify colors.
The value of the property starts with the letters hsl, followed by individual values inside
parentheses for:
# hue
This is expressed as an angle (between 0 and 360 degrees). saturation
This is expressed as a percentage.
# lightness
This is expressed as a percentage with 0% being white, 50% being normal, and 100%
being black.
The hsla color property allows you to specify color properties using hue, saturation, and
lightness as above, and adds a fourth value which represents transparency (just like the rgba
property). The a stands for: 
# alpha 
This is expressed as a number between 0 and 1.0. For example, 0.5 represents
50% transparency, and 0.75 represents 75% transparency

# Summary COLOR
1- Color not only brings your site to life, but also helps convey the mood and evokes reactions.
2- There are three ways to specify colors in CSS: RGB values, hex codes, and color names.
3- Color pickers can help you find the color you want.
4- It is important to ensure that there is enough contrast between any text and the background color (otherwise
people will not be able to read your content).
5- CSS3 has introduced an extra value for RGB colors to indicate opacity. It is known as RGBA.
6- CSS3 also allows you to specify colors as HSL values, with an optional opacity value. It is known as HSLA.


# Text
- Size and typeface of text
- Bold, italics, capitals, underlines
- Spacing between lines, words, and letters

-[X] Those that directly affect the font and its appearance (including the typeface, whether it is regular, bold or italic, and the size of the text)
-[X] Those that would have the same effect on text no matter what font you were using (including the color of text and the spacing between words and letters)
-[X] The formatting of your text can have a significant effect on how readable your pages are. As we look through these properties I will also give you some design tips on how to display your type.

# Typeface Terminology
# Serif
Serif fonts have extra details on the ends of the main strokes of the letters. These details are
known as serifs.
# Sans-Serif
Sans-serif fonts have straight ends to letters, and therefore have a much cleaner design.

# Monospace
Every letter in a monospace (or fixed-width) font is the same width. (Non-monospace fonts
have different widths.)

# Choosing a Typeface for your Website
When choosing a typeface, it is important to understand that a browser will usually only display it if it's
installed on that  user's computer.
# Serif
Serif fonts have extra details on the end of the main strokes of the letters.
Examples:
Georgia
Times
Times New Roman
# Sans-Serif
Sans-serif fonts have straight ends to letters and therefore have a much cleaner design.
Examples:
Arial
Verdana
Helvetica

# Specifying Typefaces
# font-family
The font-family property allows you to specify the typeface that should be used for
any text inside the element(s) to which a CSS rule applies.
The value of this property is the name of the typeface you want to use.
The people who are visiting your site need the typeface you have specified installed on their
computer in order for it to be displayed.
You can specify a list of fonts separated by commas so that, if the user does not have your
first choice of typeface installed, the browser can try to use an alternative font from the list.

# font-size
The font-size property enables you to specify a size for the font. There are several ways to
specify the size of a font. The most common are:
# pixels
Pixels are commonly used because they allow web designers very precise control over how much space their text
takes up. The number of pixels is followed by the letters px.
# percentages
The default size of text in browsers is 16px. So a size of 75% would be the equivalent of
12px, and 200% would be 32px. If you create a rule to make all text inside the <body> element
to be 75% of the default size (to make it 12px), and then specify another rule that indicates the
content of an element inside the <body> element should be 75% size, it will be 9px (75% of the
12px font size).

# Type Scales
This is because they are set according to a scale or ratio that was developed by European
typographers in the sixteenth century.
It is considered that this scale for type is pleasing to the eye and it has therefore changed
little in the last 400 years.
For this reason, when you are designing pages, using sizes from this scale will help them
look more attractive.
On the next page, you can see how to achieve this scale using pixels, percentages, and ems.

# More Font Choice
# @font-face
@font-face allows you to use a font, even if it is not installed on the computer of the person
browsing, by allowing you to specify a path to a copy of the font, which will be downloaded if
it is not on the user's machine. Because this technique allows a version of the font to be
downloaded to the user's computer, it is important that the license for the font permits it to
be used in this way. You add the font to your style sheet using the @font-face rule, as shown on the right.
# Font-family
This specifies the name of the font. This name can then be used as a value of the font-family
property in the rest of the style sheet (as shown in the rule for the <h1> and <h2> elements).
# src
This specifies the path to the font. In order for this technique to work in all browsers, you will
probably need to specify paths to a few different versions of the font, as shown on the next page.
# format
This specifies the format that the font is supplied in. (It's discussed in detail on the next page.)

# Bold
# font-weight
The font-weight property allows you to create bold text. There are two values that this
property commonly takes:
# normal
This causes text to appear at a normal weight.
# bold
This causes text to appear bold. In this example, you can see that the element whose class
attribute has a value of credits has been bolded.

# Italic
# font-style
If you want to create italic text, you can use the font-style property. There are three values
this property can take:
# Normal
This causes text to appear in a normal style (as opposed to italic or oblique).
# italic
This causes text to appear italic. oblique This causes text to appear
# oblique
In this example, you can see that the credits have been italicized.

# UpperCase & LowerCase
# text-transform
The text-transform property is used to change the case of text giving it one of the following
values:
# uppercase
This causes the text to appear uppercase.
# lowercase
This causes the text to appear lowercase.
# capitalize
This causes the first letter of each word to appear capitalized. In this example, the <h1>
element is uppercase, the <h2> element is lowercase, and the credits are capitalized. In the
HTML, the word by in the credits had a lowercase b

# Underline & Strike 
# text-decoration
The text-decoration property allows you to specify the following values:
# none
This removes any decoration already applied to the text.
# underline
This adds a line underneath the text.
# overline
This adds a line over the top of the text.
# line-through
This adds a line through words.
# blink
This animates the text to make it flash on and off (however this is generally frowned upon, as it is
considered rather annoying)


# Leading
# line-height
Leading (pronounced ledding) is a term typographers use for the vertical space between lines of
text. In a typeface, the part of a letter that drops beneath the baseline is called a descender,
while the highest point of a letter is called the ascender. Leading is measured from the bottom of
the descender on one line to the top of the ascender on the next.

# Letter & Word Spacing
# letter-spacing, word-spacing
Kerning is the term typographers use for the space between each letter. You can
control the space between each letter with the letter-spacing property.
It is particularly helpful to increase the kerning when your heading or sentence is
all in uppercase. If your text is in sentence (or normal) case, increasing or decreasing the
kerning can make it harder to read.
You can also control the gap between words using the word-spacing property.
When you specify a value for these properties, it should be given in ems, and it will be
added on top of the default value specified by the font.

# Alignment
# text-align
The text-align property allows you to control the alignment of text. The property can take one
of four values:
# left
This indicates that the text should be left-aligned.
# right
This indicates that the text should be right-aligned.
# center
This allows you to center text.
# justify
This indicates that every line in a paragraph, except the last line, should be set to take up the full
width of the containing box.

# Vertical Alignment
# vertical-align
The vertical-align property is a common source of confusion.
It is not intended to allow you to vertically align text in the middle of block level elements such as
<p> and <div>, although it does have this effect when used with table cells (the <td> and <th>
elements).
It is more commonly used with inline elements such as <img>, <em>, or <strong> elements.
When used with these elements, it performs a task very similar to the HTML align attribute used
on the <img> element, which you met on pages 103-106. The values it can take are:
baseline
sub
super
top
text-top
middle
bottom
text-bottom

# Indenting Text
# text-indent
The text-indent property allows you to indent the first line of text within an element.
The amount you want the line indented by can be specified in a number of ways but is usually
given in pixels or ems.
It can take a negative value, which means it can be used to push text off the browser
window. You can see this technique used in this example,
where the <h1> element uses a background image to represent the heading. The text has been
moved far to the left, off the screen. (Background images are covered on pages 413-418.)
We still want the heading text to be on the page (for search engines and those who cannot
see the image), but we cannot have it displayed on top of the logo or it will be unreadable. By
pushing it 9,999 pixels to the left, it is way out of sight but still in the HTML code.


# CSS3: Drop Shadow
# text-shadow
The text-shadow property has become commonly used despite lacking support in all browsers.
It is used to create a drop shadow, which is a dark version of the word just behind it and
slightly offset. It can also be used to create an embossed effect by adding a shadow that is slightly
lighter than the text.
The value of this property is quite complicated because it can take three lengths and a color for
the drop shadow.
The first length indicates how far to the left or right the shadow should fall.
The second value indicates the distance to the top or bottom that the shadow should fall.
The third value is optional and specifies the amount of blur that should be applied to the drop
shadow.
The fourth value is the color of the drop shadow.

# First Letter or Line
# first-letter, :first-line
You can specify different values for the first letter or first line of
text inside an element using :first-letter and :first-line.
Technically these are not properties. They are known as pseudo-elements.
You specify the pseudo-element at the end of the selector, and then specify the declarations as
you would normally for any other element.

# Styling Links
# link, :visited
Browsers tend to show links in blue with an underline by default, and they will change
the color of links that have been visited to help users know which pages they have been to.
In CSS, there are two pseudoclasses that allow you to set different styles for links that
have and have not yet been visited.
# link
This allows you to set styles for links that have not yet been visited.
# visited
This allows you to set styles for links that have been clicked on.
They are commonly used to control colors of the links and also whether they are to appear
underlined or not.
On the left, you can see that visited links are shown in a different color to help visitors
know what they have alreadyseen.

# Responding to Users
# hover, :active, :focus
There are three pseudo-classes that allow you to change the appearance of elements when a
user is interacting with them.
# hover
This is applied when a user hovers over an element with a pointing device such as a mouse.
This has commonly been used to change the appearance of links and buttons when a user
places their cursor over them. It is worth noting that such events do not work on devices that use
touch screens (such as the iPad) because the screen is not able to tell when someone is hovering
their finger over an element.
# active
This is applied when an element is being activated by a user; for example, when a button is being
pressed or a link being clicked.
Sometimes this is used to make a button or link feel more like it is being pressed by changing the
style or position of the element slightly.
# focus
This is applied when an element has focus. Any element that you can interact with, such as a
link you can click on or any form control can have focus.

