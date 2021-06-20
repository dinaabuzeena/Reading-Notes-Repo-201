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
  
  < sup >
    
The < sup > element is used to contain characters that should be superscript such as the suffixes of dates or mathematical concepts like raising a number to a
power suchas 22

    
< sub >
  
The < sub > element is used to contain characters that should be subscript. It is commonly used with foot notes or chemical formulas such as H20.
  
  
 ** White Space**
  
  In order to make code easier to   read, web page authors often add extra spaces or start some elements on new lines.
When the browser comes across two or more spaces next to each other, it only displays one space.
Similarly if it comes across a line break, it treats that as a single space too. This is known as white space collapsing
  
  
  **Line Breaks & Horizontal Rules**
  
< br />
  
As you have already seen, the browser will automatically show each new paragraph or heading on a new line. But if you wanted to add a line break inside the
middle of a paragraph you canuse the line break tag < br />
  
  
  
  
   <hr />
  
To create a break between themes — such as a change of topic in a book or a new scene in a play — you can add a horizontal rule between sections
using the < hr /> tag
  
  
  
  
  **Strong & Emphasis**
  
  <  strong  >
    
The use of the < strong > element indicates that its content has strong importance.
For example, the words contained in this element might be said with strong emphasis.
    
By default, browsers will show the contents of a < strong > element in bold.
    
    
    
  < em >
      
The < em > element indicates emphasis that subtly changes the meaning of a sentence.
By default browsers will show the contents of an  < em > element in italic.

  
    
  **Quotations**
      
  < blockquote >
    
The < blockquote  > element is used for longer quotes that take up an entire paragraph. 
    
   
< q >
  
The <q> element is used for shorter quotes that sit within a paragraph. Browsers are supposed to put quotes around the <q> element, however Internet Explorer does not —
therefore many people avoidusing the < q > element.
  
  
 **Abbreviations & Acronyms**
  
  < abbr  > 
    
If you use an abbreviation or an acronym, then the <abbr> element can be used. A title attribute on the opening tag isused to specify the full term.


    
 **Citations & Definitions*
    
    <cite>
      
When you are referencing apiece of work such as a book,film or research paper, the<cite> element can be usedto indicate where the citation isfrom.
In HTML5, <cite> should notreally be used for a person'sname — but it was allowed inHTML 4, so most people arelikely to continue to use it.
    
    <dfn>
The first time you explain somenew terminology (perhaps anacademic concept or somejargon) in a document, it isknown as the defining instanceof it.
The <dfn> element is used toindicate the defining instance of a new term.
    
      
      
      
  # HTML5: Adding HTML5 Audio to Your Pages
 **audio**
      
chapter-09/adding-html5-audio.html HTML HTML5 introduced the <audio> element to include audio files in your pages. As with HTML5
video, browsers expect different formats for the audio. The <audio> element has a number of attributes which allow you to control audio playback: 
        
**src**
      
This attribute specifies the path
to the audio file.
        
**controls**
      
This attribute indicates whether the player should display controls. If you do not use this attribute, no controls will be shown by default. You can also
specify your own controls using JavaScript.
        
**autoplay**
The presence of this attribute indicates that the audio should start playing automatically. (It is considered better practice to let visitors choose to play audio.)
HTML5: Adding HTML5 Audio to Your Pages
      
      
**preload**
This attribute indicates what the browser should do if the player is not set to autoplay. It can have the same values we saw on page 214 for the <video> element.
      
      
**loop**
This attribute specifies that the audio track should play again once it has finished.
      
      
# HTML5: Multiple Audio Sources
< source >
      
It is possible to specify more than one audio file using the <source> element between the opening <audio> and closing </audio> tags (instead of the src attribute 
on the opening <audio> tag).
      
# Summary
FLASH, VIDEO & AUDIO
      
-[x]  Flash allows you to add animations, video and audio to
the web.
-[x]  Flash is not supported on iPhone or iPad.
      
-[x]  HTML5 introduces new <video> and <audio> elements for adding video and audio to web pages, but these are only supported in the latest browsers.
      
-[x]  Browsers that support the HTML5 elements do not all support the same video and audio formats, so you need to supply your files in different formats to ensure
    that everyone can see/hear them
      
      

