<link rel="preload" as="style" href="https://actwu.github.io/md.css"/>  
<link rel="stylesheet" href="https://actwu.github.io/md.css"/>  

# JavaScript Guideline

This is a JavaScript guideline for learning.
It focuses on clean, fast, and modern browser-side coding.
All examples follow a direct, no-frills style.

***This is based on web4now guideline.***

---

## File Extension

```javascript
// Save JavaScript files with `.js` extension
```

## Comment

```javascript
// Single line comment
```

---

## Variable

```javascript
variable = value;
```

---

## Table (Array)

```javascript
table = ["item1", "item2"];
```

You can assign tables to variables or include variables inside tables.

```javascript
table_in_var = table;

var_in_table = [var1, var2, var3];
```

---

## Act / Action (Function)

Functions are written as actions. Sub-actions are attached as properties.

```javascript
act = () => {};
```

### Sub Act
```javascript
sub.act = () => {};
```

### Temporal (IIFE)

Temporal are temporary and run immediately this is also use to open system of js.

```javascript
(() => {
  
})();
```

---

## Loop

Use `setInterval` for repeated actions.
This is part of the browser’s system and is reliable.

```javascript
setInterval(() => {
  // repeated code
}, milliseconds);
```

Use `setTimeout` for delayed actions.

```javascript
setTimeout(() => {
  // delayed code
}, milliseconds);
```

---

## Reason (If / Else) 

Use `? :` for short conditionals.

```javascript
condition ? doThis() : doThat();
```

Example:

```javascript
el.exists
? (() => {
// if true
})()

: (() => {
// if false
)();
```

---

## Replace

For replacing characters or rebuilding strings:

```javascript
string.split('').join('');
```

---

## insertAdjacentHTML

The browser already provides `insertAdjacentHTML`.
You do not need `.append()` or `.innerHTML += …`.
This is clean, safe, and fast.

Usage:

```javascript
el.insertAdjacentHTML('beforeend', '<span>content</span>');
```

It supports four positions:

* `'beforebegin'` — before the element itself
* `'afterbegin'` — just inside the element, before its first child
* `'beforeend'` — just inside the element, after its last child
* `'afterend'` — after the element itself

Example:

```javascript
el.insertAdjacentHTML('beforeend', '<section>New</section>');
```

---

## Attributes

Use literal attributes to store state or meaning.
There is no need to use `data-*` attributes — modern browsers support literal attributes and they are faster.

Example:

```html
<section state="active"></section>
```

Do not overuse `<div>`. Use proper elements like `<section>`, `<header>`, `<main>`, `<footer>`, `<button>`, `<input>`.

---

## Events

For clean and fast code, write events directly in HTML.
This reduces overhead and improves performance.

```html
<input oninput="myAction()" />
<main onmousedown="myAction()"></main>
<body onkeydown="myAction()"></body>
```

---

## toggleAttribute

Use the browser’s built-in `toggleAttribute()` method.

```javascript
el.toggleAttribute('state');
```

---

## Summary

* Do not use `class` keyword or `.classList`.
* Do not use `data-*` attributes — use literal attributes.
* Avoid unnecessary `<div>` elements — use meaningful HTML tags.
* Use native `insertAdjacentHTML()` — no wrappers needed.
* Write event handlers directly in HTML (`oninput`, `onmousedown`, `onkeydown`).
* Use native `toggleAttribute()`.
* Use `setInterval` and `setTimeout` for timing.
* Keep your code clean and minimal.

---

lol
