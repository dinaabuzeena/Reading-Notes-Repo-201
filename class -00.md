HTML & CSS
Design and build Websites
No part of this publication may be reproduced, stored in a retrieval system or transmitted in any form or by any means, electronic, mechanical,
photocopying, recording, scanning or otherwise, except as permitted under Sections 107 or 108 of the 1976 United States Copyright Act,
without either the prior written permission of the Publisher, or authorization through payment of the appropriate per-copy fee to the
Copyright Clearance Center, 222 Rosewood Drive, Danvers, MA 01923, (978) 750-8400, fax (978) 646-8600. Requests to the Publisher for
permission should be addressed to the Permissions Department, John Wiley & Sons, Inc., 111 River Street, Hoboken, NJ 07030, (201) 748-
6011, fax (201) 748-6008, or online at http://www.wiley.com/go/permissions.
Limit of Liability/Disclaimer of Warranty: The publisher and the author make no representations or warranties with respect to the
accuracy or completeness of the contents of this work and specifically disclaim all warranties, including without limitation warranties of
fitness for a particular purpose. No warranty may be created or extended by sales or promotional materials. The advice and strategies
contained herein may not be suitable for every situation. This work is sold with the understanding that the publisher is not engaged in
rendering legal, accounting, or other professional services. If professional assistance is required, the services of a competent professional
person should be sought. Neither the publisher nor the author shall be liable for damages arising herefrom. The fact that an organization
or Web site is referred to in this work as a citation and/or a potential source of further information does not mean that the author or the
publisher endorses the information the organization or website may provide or recommendations it may make. Further, readers should be
aware that Internet websites listed in this work may have changed or disappeared between when this work was written and when it is read.
For general information on our other products and services please contact our Customer Care Department within the United States at (877)
762-2974, outside the United States at (317) 572-3993 or fax (317) 572-4002.
Wiley also publishes its books in a variety of electronic formats. Some content that appears in print may not be available in electronic books.
Library of Congress Control Number: 2011932082
Trademarks: Wiley and the Wiley logo are trademarks or registered trademarks of John Wiley & Sons, Inc. and/or its
affiliates, in the United States and other countries, and may not be used without written permission. All other trademarks are
the property of their respective owners. John Wiley & Sons, Inc. is not associated with any product or vendor mentioned in
this book.


# Introduction
1-About this book
2- How the web works
3- Learning from other pages

Firstly, thank you for picking up this book. It has been written with two very different types of people in mind:

● Those who want to learn how to design and build websites
from scratch
● Anyone who has a website (that may be built using a content management system, blogging software, or an e-commerce platform) and wants more control over the
appearance of their pages

The only things you need in order to use this book are a computer with a web browser and a text editor (such as Notepad, which comes with Windows, or TextEdit, which
comes with Macs).

# The Structure of This Book
1: HTML
We will spend the first chapter looking at how HTML is used to create web pages. You will see
that you start by writing downth ds you want to appear on your page. You then add tags
or elements to the words so that the browser knows what is a heading, where a paragraph
begins and ends, and so on.
The rest of this section introduces the tags you have at your disposal to create web
pages, grouped into chapters on: text, lists, links, images, tables, forms, video audio and flash, and miscellaneous elements.

2: CSS
We start this section with a chapter that explains how CSS uses rules to enable you to
control the styling and layout of web pages. We then go on to look at the wide variety of CSS
properties you can use in your CSS rules. These properties generally fall into one of two
categories:
Presentation: How to control things like the color of text, the fonts you want to use and the
size of those fonts, how to add background colors to pages (or parts of a page), and how to add
background images.
Layout: How to control where the different elements are positioned on the screen. You
will also learn several techniques that professionals use to make their pages more attractive.

3: Practical
We end up with some helpful information that will assist you in building better websites.
We look at some new tags that will be introduced in HTML5 to help describe the structure of
your pages. HTML5 is the latest version of HTML (still under development at the time of
writing). Before learning about these elements, you need a good grasp of how CSS is used to
control the design of web pages.
There is a chapter that talks you through a design process that you might like to follow when
creating a new website.


# Structure
1-Understanding structure
2- Learning about markup
3- Tags and elements

Many web pages act like electronic versions of these
documents. For example, newspapers show the same stories
in print as they do on websites; you can apply for insurance
over the web; and stores have online catalogs and e-commerce
facilities.
In all kinds of documents, structure is very important in helping
readers to understand the messages you are trying to convey
and to navigate around the document. So, in order to learn how
to write web pages, it is very important to understand how to
structure documents. In this chapter you will:
1- See how HTML describes the structure of a web page
2- Learn how tags or elements are added to your document
3- Write your first web page

# Attributes Tell Us More About Elements
Attributes provide additional information about the contents of an element. They appear
on the opening tag of the element and are made up of two parts: a name and a value,
separated by an equals sign.


Body, Head & Title

<body>
You met the <body> element in the first example we created.
Everything inside this element ismshown inside the main browser window.

<head>
Before the <body> element you will often see a <head> element.
This contains information about the page (rather than
information that is shown within the main part of the browser window that is highlighted in
blue on the opposite page).
You will usually find a <title> element inside the <head> element.

<title>
The contents of the <title> element are either shown in thetop of the browser, above where
you usually type in the URL of the page you want to visit, or on the tab for that page (if your
browser uses tabs to allow you to view multiple pages at the same time).