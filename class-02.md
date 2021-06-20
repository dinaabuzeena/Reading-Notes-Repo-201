# Code in a Content Management System
- management system, blogging platform, or e-commerce application, you will probably log into a special administration section of the website to controlit.
The tools provided in the administration sections of these sites usually allow you to edit parts of the page rather than the entire page, which meansyou will rarely see
the <html>,<head>, or <body> elementsde in a Content Management System.
  
- The advantage of this approach is that people who do not know how to write web pages can add information to a website and it is also possible to change
the presentation of something in the template, and it will automatically update every page that uses that template. If you imagine an e-commerce store with 1,000 items for sale.
  
 - Some content management systems offer tools that also allow you to edit the template files. If you do try to edit template files you need to checkthe documentation
 for your CMSas they all differ from each other.You need to be careful when editing template files because if you delete the wrong piece of code or add something in the
wrong place the site may stop working entirely.
  
  
  
 **Looking at How Other sites are Built**
  
These days there are many more books and online tutorials that teach HTML, but you can still look at the code that a web server sends to you. To try this
out for yourself, simply go to the sample code for this chapter, at www.htmlandcssbook.com/ code/ and click on the link called "View Source."
Once you have opened this page, you can look for the View menu in your browser, and select the option that says Source or View source. (The title changes
depending on what browser you are using.)
You should see a new window appear, and it will contain the source code that was used to create this page.
You can see this result in the photograph on the right. The page you see is the window at the top; the code is below.
  
  
**In this chapter** we focus on how to add markup to the text that
appears on your pages. You will learn about:
● Structural markup: the elements that you can use to
describe both headings and paragraphs
● Semantic markup: which provides extra information; such
as where emphasis is placed in a sentence, that something
you have written is a quotation (and who said it), the
meaning of acronyms, and so on
  
  
  **Headings*
  
HTML has six "levels" of
headings:
  
1- h1 is used for main headings
  
2- h2 is used for subheadings
  
3- If there are further sections
under the subheadings then the
h3 element is used, and so
on...
  
  
  **Paragraphs**
  To create a paragraph, surround the words that make up the paragraph with an opening < p > tag and closing </ p > tag.
  
  
  
  **Bold & Italic**
  
  < b > 
    
 By enclosing words in the tags < b > and < /b > we can make characters appear bold.
The < b > element also represents a section of text that would be presented in a visually different way (for example key words in aparagraph) although the use of
the < b > element does not implyany additional meaning.
    
    
  <i>
    
By enclosing words in the tags <i> and </i> we can make characters appear italic. The <i> element also represents a section of text that would besaid in a 
differen way from surrounding content — such as technical terms, names of ships, foreign words, thoughts, or other terms that would usually be italicized.

  
  
  **Superscript & Subscrip**
  
  <sup>
    
The <sup> element is used to contain characters that should be superscript such as the suffixes of dates or mathematical concepts like raising a number to a
power suchas 22

    
<sub>
  
The <sub> element is used to contain characters that should be subscript. It is commonly used with foot notes or chemical formulas such as H20.
  
  
 ** White Space**
  
  In order to make code easier to   read, web page authors often add extra spaces or start some elements on new lines.
When the browser comes across two or more spaces next to each other, it only displays one space.
Similarly if it comes across a line break, it treats that as a single space too. This is known as white space collapsing
  
  
  **Line Breaks & Horizontal Rules**
  
  
<br />
  
As you have already seen, the browser will automatically show each new paragraph or heading on a new line. But if you wanted to add a line break inside the
middle of a paragraph you canuse the line break tag <br />.
  
  
  
  <hr />
  
To create a break between themes — such as a change of topic in a book or a new scene in a play — you can add a horizontal rule between sections
using the <hr /> tag
  
  
  
  **Strong & Emphasis**
  
  <strong>
    
The use of the <strong> element indicates that its content has strong importance.
For example, the words contained in this element might be said with strong emphasis.
    
By default, browsers will show the contents of a <strong> element in bold.

  
  
  
  
