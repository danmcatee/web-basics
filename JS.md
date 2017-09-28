---
title: Web basics | JavaScript
separator: <!-- s -->
verticalSeparator: ---
theme: solarized
---
# Web Basics
### JavaScript
<!-- s -->
# Basic syntax
---
## Variables

```js
var integer = 42;
var float   = 1.4;
var string  = "Hello world!";
var array   = [1,2,3];
```
 <!-- .element: class="fragment" data-fragment-index="1" -->

 - Every common browser has a JavaScript console!
 <!-- .element: class="fragment" data-fragment-index="2" -->

---
## Operations

```js
var sum = integer + float;
// 43.4
var text = string + " (and cheeze to come!)";
// "Hello world! (and cheeze to come!)"
```
 <!-- .element: class="fragment" data-fragment-index="1" -->
---
## Output

```js
console.log("hi"); // outputs "hi"
console.log(sum); //  outputs "43.4"
```

 <!-- .element: class="fragment" data-fragment-index="1" -->
---
## &lt;script&gt; tag

```html
<script>
    console.log(
        "js got executed when your browser parsed this page!"
    );
</script>
```
 <!-- .element: class="fragment" data-fragment-index="1" -->

<!-- s -->

# JQuery

> jQuery is a fast, small, and feature-rich JavaScript library. It makes things like HTML document traversal and manipulation, event handling, animation, and Ajax much simpler with an easy-to-use API that works across a multitude of browsers. [...]

 <!-- .element: class="fragment" data-fragment-index="1" -->

---

# Basic usage

 - get the code
  <!-- .element: class="fragment" data-fragment-index="1" -->

 ```html
 <script 
    src="https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js"
 ></script>
 ```
  <!-- .element: class="fragment" data-fragment-index="2" -->
 
 - DOM Traversal
 <!-- .element: class="fragment" data-fragment-index="3" -->
 - DOM Manipulation
 <!-- .element: class="fragment" data-fragment-index="4" -->


---
## DOM Traversal

 - with CSS selectors

```js
$("input")
```

<!-- .element: class="fragment" data-fragment-index="1" -->

```js
$("#cheese")
```

<!-- .element: class="fragment" data-fragment-index="2" -->

```js
$(".fire-button")
```

<!-- .element: class="fragment" data-fragment-index="3" -->

```js
$("a:visited")
```

<!-- .element: class="fragment" data-fragment-index="4" -->

```js
$("input[type='checkbox']")
```

<!-- .element: class="fragment" data-fragment-index="5" -->
---
## Document manipulation

 - change markup

 <!-- .element: class="fragment" data-fragment-index="1" -->

```js
$("#cheese-feed").append("more cheese");
```

<!-- .element: class="fragment" data-fragment-index="2" -->

 - change style

 <!-- .element: class="fragment" data-fragment-index="3" -->

```js
$('footer').css('background-color', 'orange');
```

<!-- .element: class="fragment" data-fragment-index="4" -->
