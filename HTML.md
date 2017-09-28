---
title: Web Basics Workshop
separator: <!--s-->
verticalSeparator: <!--v-->
theme: solarized
revealOptions:
    transition: 'fade'
---

# HTML BASICS

<!--s-->

### Overview

* Markup language is used to structure the contents of a web page
<!-- .element: class="fragment" data-fragment-index="1" -->

*  It is NOT a programming language
<!-- .element: class="fragment" data-fragment-index="2" -->

* Current standard is HTML 5
<!-- .element: class="fragment" data-fragment-index="3" -->

* HTML is NOT used for design or layout purposes (-> CSS)
<!-- .element: class="fragment" data-fragment-index="4" -->

<!--s-->

### Basics

* an HTML document consists mainly of a head and a body
<!-- .element: class="fragment" data-fragment-index="1" -->
* the head part is for providing meta information about the document (title, char-encoding, ...)
<!-- .element: class="fragment" data-fragment-index="2" -->
* the body part contains everything that is being displayed by the browser
<!-- .element: class="fragment" data-fragment-index="3" -->

<!--s-->

### Example

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

<!--s-->

### Tags

Tags are used to declare any kind of element (text, list, image, ...).
<!-- .element: class="fragment" data-fragment-index="1" -->
There are two kinds of tags:
<!-- .element: class="fragment" data-fragment-index="2" -->
* Tags that have closing counterpart <!-- .element: class="fragment" data-fragment-index="3" --> `<html></html>`
<!-- .element: class="fragment" data-fragment-index="4" -->
* Tags that are self enclosing <!-- .element: class="fragment" data-fragment-index="5" --> `<input/>`
<!-- .element: class="fragment" data-fragment-index="6" -->
* Nesting multiple tags creates a hierarchical structure:
<!-- .element: class="fragment" data-fragment-index="7" -->

<!--s-->

### Example

```html
<html> ... </html> 
<!-- These provide a 'frame' for everything else -->
<head> ... </head> 
<!-- These declare the head part -->
<body> ... </body> 
<!-- ...and these the body part -->
<h1> Title </h1> 
<!-- Titles! and there are more: h2, h3 -->
<p> Lorem ips.. </p> 
<!-- Paragraphs for blocks of plain text -->
<div> ... </div> 
<!-- A div tag, used very, very often. Especially for grouping elements -->
<a href="catgif.jpg"> ... </a> 
<!-- A Link! The href part defines where it links to -->
<input type="text"/> 
<!-- Declare some kind of user input, in this case a text input. Does not have a closing tag! -->
 ```

 <!--s-->

### Attributes

Attributes can be added to a tag in order to define an aspect of its functionality. There are four kinds of attributes:
 <!-- .element: class="fragment" data-fragment-index="1" -->

<!--s-->

* attributes with predefined values


```html
<input type="text"> 
<!-- The attribute is the 'type="text"' part.  -->
<input type="checkbox"> 
<!-- This is also a valid attribute for an input element -->
<input type="someinput"> 
<!-- This wont do!>
```

<!--s-->

* attributes with values that need to match some format, but can be chosen freely

```html
<input type="text" maxlenght="10"> 
<!-- Multiple attributes are possible! 
This input element is of the 'text' kind,
but only allows 10 characters as input. -->
```
<!--v-->

```html
<input type="text" maxlength="100"> 
<!-- But you can make it a 100 as well! 
As long as the value of the attribute is 
a positive integer, it doesn't matter. -->
```

<!--v-->

```html
<input type="text" maxlength="unicorn"> 
<!-- Won't do either. unicorn is not an integer -->
```

<!--s-->

* attributes with values that don't need to match any format

```html
<p title="This can be literally everything: $$cheesecake123"> ... </p>
```

<!--s-->

* standalone attributes

```html
<input type="text" readonly> 
<!-- Because of the 'readonly' attribute,
 a user won't be able to modify the text 
 in the input field -->
```

<!--s-->

# Important Attributes

<!--s-->

The 'lang' attribute declares the language. This is important for accessability applications and search engines.
```html
<html lang="en-US">
```

<!--s-->

The 'href' attribute specifies the link address in an anchor element (A plain link)
```html
<a href="https://www.unicorns.com/img/rainbow.jpg"> This text will be clickable! </a>
```

<!--s-->

The 'alt' attribute specifies an alternative text to be used, when an image cannot be displayed.The value of the attribute can be read by screen readers. This way, someone "listening" to the webpage, e.g. a blind person, can "hear" the element.
```html
<img src="unicorn.jpg" alt="The picture shows a unicorn">
```

<!--s-->

The 'id' attribute specifies a unique id for an html element. This is useful for pointing to style in a style sheet (-> CSS, we'll get to that later)
```html
<h1 id="title-one">Hello Title!</h1>
```

<!--s-->

Similar, the 'class' attribute also makes possible to group one or more elements under a class name. Again, this is needed when working with CSS and/or JavaScript
```html
<h1 class="intro">Header 1</h1>
<p>A paragraph.</p>
<p class="important">Note that this is an important paragraph. :)</p>
```

<!--s-->

### Sources
* www.w3schools.com
* wiki.selfhtml.org
