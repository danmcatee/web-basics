# HTML BASICS

## Overview

* Markup language is used to structure the contents of a web page
*  It is NOT a programming language
* Current standard is HTML 5
* HTML is NOT used for design or layout purposes (-> CSS)

## Basics

* an HTML document consists mainly of a head and a body
* the head part is for providing meta information about the document (title, char-encoding, ...)
* the body part contains everything that is being displayed by the browser

```html
<!Doctype html>
<html lang="en">
  <head>
    <meta charset="utf8">
    <title>Some Title</title>
  </head>
  <body>
    <h1>Element</h1>
    <!-- This is a comment! -->
  </body>
</html>
```

## Tags

Tags are used to declare any kind of element (text, list, image, ...).
There are two kinds of tags:
* Tags that have closing counterpart (`<html></html>`)
* Tags that are self enclosing (`<input/>`)
Nesting multiple tags creates a hierarchical structure:

```html
 <html> ... </html> <!-- These provide a 'frame' for everything else -->
<head> ... </head> <!-- These declare the head part -->
<body> ... </body> <!-- ...and these the body part -->
<h1> Title </h1> <!-- Titles! and there are more: h2, h3 -->
<p> Lorem ips.. </p> <!-- Paragraphs for blocks of plain text -->
<div> ... </div> <!-- A div tag, used very, very often. Especially for grouping elements -->
<a href="catgif.jpg"> ... </a> <!-- A Link! The href part defines where it links to -->
<input type="text"/> <!-- Declare some kind of user input, in this case a text input. Does not have a closing tag! -->
 ```

## Attributes

Attributes can be added to a tag in order to define an aspect of its functionality. There are four kinds of Attributes:
* attributes with predefined values
```html
<input type="text"> <!-- The attribute is the 'type="text"' part.  -->
<input type="checkbox"> <!-- This is also a valid attribute for an input element -->
<input type="someinput"> <!-- This wont do!>
```
* attributes with values that need to match some format, but can be chosen freely
```html
<input type="text" maxlenght="10"> <!-- Multiple attributes are possible! This input element is of the 'text' kind, but only allows 10 characters as input. -->
<input type="text" maxlength="100"> <!-- But you can make it a 100 as well! As long as the value of the attribute is a positive integer, it doesn't matter. -->
<input type="text" maxlength="unicorn"> <!-- Won't do either. unicorn is not an integer -->
```
* attributes with values that don't need to match any format
```html
<p title="This can be literally everything: $$cheesecake123"> ... </p>
```
* standalone attributes
```html
<input type="text" readonly> <!-- Because of the 'readonly' attribute, a user won't be able to modify the text in the input field -->
```

## Important Attributes

The 'lang' attribute declares the language. This is important for accessability applications and search engines.
```html
<html lang="en-US">
```
The 'href' attribute specifies the link address in an anchor element (A plain link)
```html
<a href="https://www.unicorns.com/img/rainbow.jpg"> This text will be clickable! </a>
```
The 'alt' attribute specifies an alternative text to be used, when an image cannot be displayed.The value of the attribute can be read by screen readers. This way, someone "listening" to the webpage, e.g. a blind person, can "hear" the element.
```html
<img src="unicorn.jpg" alt="The picture shows a unicorn">
```
The 'id' attribute specifies a unique id for an html element. This is useful for pointing to style in a style sheet (-> CSS, we'll get to that later)
```html
<h1 id="title-one">Hello Title!</h1>
```
Similar, the 'class' attribute also makes possible to group one or more elements under a class name. Again, this is needed when working with CSS and/or JavaScript
```html
<h1 class="intro">Header 1</h1>
<p>A paragraph.</p>
<p class="important">Note that this is an important paragraph. :)</p>
```

## Sources
* www.w3schools.com
* wiki.selfhtml.org
