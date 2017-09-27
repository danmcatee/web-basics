# HTML BASICS

## Overview

* Markup language used to structure the contents of a web page
* Is NOT a programming language
* Current standard is HTML 5
* HTML is NOT used for design or layout purposes (-> CSS)

## Basics

* an HTML document consists of a head and a body
* the head part is for providing meta information about the document (title, char-encoding, ...)
* the body part contains everything that is being displayed by the browser

## Tags

Tags used to declare any kind of element (text, list, image, ...).
There are two kinds of tags:
* Tags that have closing counterpart (`<html></html>`)
* Tags that are self enclosing (`<input/>`)
Nesting multiple tags creates a hierarchical structure:

```html
 <html>
   <head>
       
   </head>
   <body>
       
   </body>
 </html>
 ```

## Common Tags

* `<html></html>`
* `<head></head>`
* `<body></body>`
* `<h1></h1>`, `<h2></h2>`, `<h3></h3>` Headlines that differ in size (`<h1>` being the biggest)
* `<p></p>` a paragraph of text
* `<div>` often used to layout a web page
* `<a href=""></a>` the anchor tag with href attribute is used to create a link
* `<input>` the input tag is used to create an input element  that a user can use

## Attributes

Attributes can be added to a tag in order to define an aspect of its functionality. There are four kinds of Attributes:
* attributes with predefined values (`<input type="text">`)
* attributes with values that need to match some format, but can be chosen freely (`<input type="text" maxlenght="10">`)
* attributes with values that don't need to match any format (`<p title="This can be anything">`)
* standalone attributes (`<input type="text" readonly>`)  

## Common Attributes

* the id attribute specifies a unique id for an html element. This is useful for pointing a style from a stylesheet to the element, or for manipulating it with JavaScript
* the class attribute makes it possible to define equal styles for elements with the same class name.
