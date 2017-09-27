# The General Rule
```css
selector {
  property: value;
  anotherProperty: value;
}
``` 

---

# Examples
```css
/*Make All h1's purple and 56px font*/
h1 {
  color: purple;
  font-size: 56px;
}

/*Give All img's a 3px red border*/

img {
  border-color: red;
  border-width: 3px;
}
```

---

# Where do we write our styles 
Inline:
```html
<h3 style="color: pink;">blah blah blah </h3>
<h3 style="color: pink;">knock knock </h3>

<p style="color: yellow;">blah blah blah </p>
```
StyleTag:
```html
<html>
<head>
    <title>About Rusty</title>
    <style type="text/css">
        li {
	    color: red;
	}
    </style>
</head>
````

## Thats a bad Idea!!!

---

# Write your CSS in a seperate file

HTML File:
```html
<!DOCTYPE html>
<html>
<head>
    <title>Demo Page</title>
    <link rel="stylesheet" type="text/css" href="app.css">
</head>
<body>
	
</body>
</html>
```

CSS File:
```css
h1 {
  color: purple;
}

h3 {
 color: pink;
}
```

***

# Colors in CSS

## Built in colors

```css
h1 {
  color: red;
}

h2 {
  color: cornflowerBlue;
}

h3 {
  color: darkOrchid;
}
```

```html
<h1>I'm a h1</h1>
<h2>I'm a h2</h2>
<h3>I'm a h3</h3>
````

<h1 style="color: red">I'm a h1</h1>
<h2 style="color: cornflowerBlue">I'm a h2</h2>
<h3 style="color: darkOrchid">I'm a h3</h3>

---

## Hexadecimal

```css
h1 {
  color: #ffffff;
}

h2 {
  color: #4B0082;
}

h3 {
  color: #FF1493;
}
```

```html
<h1>I'm a h1</h1>
<h2>I'm a h2</h2>
<h3>I'm a h3</h3>
````

<h1 style="color: #ffffff">I'm a h1</h1>
<h2 style="color: #4B0082">I'm a h2</h2>
<h3 style="color: #FF1493">I'm a h3</h3>

---

## RGB

```css
h1 {
  color: rgb(0,255,0);
}

h2 {
  color: rgb(100, 0, 100);
}

h3 {
  color: rgb(11, 99, 150);
}
````

```html
<h1>I'm a h1</h1>
<h2>I'm a h2</h2>
<h3>I'm a h3</h3>
````

<h1 style="color: rgb(0,255,0)">I'm a h1</h1>
<h2 style="color: rgb(100, 0, 100)">I'm a h2</h2>
<h3 style="color: rgb(11, 99, 150)">I'm a h3</h3>

---

## RGBA

```css
h1 {
  color: rgba(11, 99, 150, 1);
}

h2 {
  color: rgba(11, 99, 150, .6);
}

h3 {
  color: rgba(11, 99, 150, .2);
}
````

```html
<h1>I'm a h1</h1>
<h2>I'm a h2</h2>
<h3>I'm a h3</h3>
````

<h1 style="color: rgba(11, 99, 150, 1)">I'm a h1</h1>
<h2 style="color: rgba(11, 99, 150, .6)">I'm a h2</h2>
<h3 style="color: rgba(11, 99, 150, .2)">I'm a h3</h3>

---

## Color and Background

```css
div{
  background: #3498db;
}

p {
  color: #ecf0f1;
}
````

```html
<div>
  <p>Hello</p>
  <p>Goodbye</p>
</div>
```
<div style="background: #3498db">
  <p style="color: #ecf0f1">Hello</p>
  <p style="color: #ecf0f1">Goodbye</p>
</div>

---

# CSS Selectors

## Element Selectors

```html
<div>
  <p>You say yes</p>
  <p>I say no</p>
</div>

<div>
  <p>You say goodbye</p>
  <p>I say hello </p>
</div>
````

```css
div{
  background: purple;
}

p {
  color: yellow;
}
````

<div style="background: purple">
  <p style="color: yellow">You say yes</p>
  <p style="color: yellow">I say no</p>
</div>

<div style="background: purple">
  <p style="color: yellow">You say goodbye</p>
  <p style="color: yellow">I say hello </p>
</div>

---

## ID Selector

```html
<div>
  <p>You say yes</p>
  <p>I say no</p>
</div>

<div>
  <p>You say goodbye</p>
  <p id="special">I say hello </p>
</div>
````

```css
div{
  background: purple;
}

#special {
  color: yellow;
}
````

<div style="background: purple">
  <p>You say yes</p>
  <p>I say no</p>
</div>

<div style="background: purple">
  <p>You say goodbye</p>
  <p style="color: yellow">I say hello </p>
</div>

---

## Class Selector

```html
<div>
  <p class="highlight">You say yes</p>
  <p>I say no</p>
</div>

<div>
  <p class="highlight">You say goodbye</p>
  <p>I say hello </p>
</div>
````

```css
div{
  background: purple;
}

.highlight {
  color: yellow;
}
````

<div style="background: purple">
  <p style="color: yellow">You say yes</p>
  <p>I say no</p>
</div>

<div style="background: purple">
  <p style="color: yellow">You say goodbye</p>
  <p>I say hello </p>
</div>

---

# Box Model

- Content
- Padding
- Border
- Margin
