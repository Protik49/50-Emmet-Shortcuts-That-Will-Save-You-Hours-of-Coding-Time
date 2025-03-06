# 50 Emmet Shortcuts That Will Save You Hours of Coding Time


![Emmet Logo](https://unsplash.com/photos/npxXWgQ33ZQ/download?ixid=M3wxMjA3fDB8MXxzZWFyY2h8Mnx8Y29kaW5nfGVufDB8fHx8MTcxNjE0NzE0OHww&force=true&w=1920)

## Introduction

Emmet is a powerful toolkit for web developers that can significantly improve your HTML and CSS workflow. Originally known as Zen Coding, Emmet uses simple expressions to generate HTML, XML, and CSS code, allowing you to write code faster and more efficiently. This guide covers 50 essential Emmet techniques that every web developer should know.

## Table of Contents

1. [HTML Basics](#html-basics)
2. [Advanced HTML Techniques](#advanced-html-techniques)
3. [CSS Techniques](#css-techniques)
4. [Workflow Optimization](#workflow-optimization)
5. [Framework-Specific Techniques](#framework-specific-techniques)
6. [Custom Configurations](#custom-configurations)
7. [Resources and Further Learning](#resources-and-further-learning)

## HTML Basics

### 1. Element Creation

The most basic Emmet technique is creating HTML elements by simply typing their name.

**Syntax:** `div`  
**Output:** `<div></div>`

**Example:**
```html
p → <p></p>
```

### 2. Nested Elements

Create nested elements using the child operator `>`.

**Syntax:** `div>p`  
**Output:** `<div><p></p></div>`

**Example:**
```html
ul>li → <ul><li></li></ul>
```

### 3. Sibling Elements

Create sibling elements using the adjacent sibling operator `+`.

**Syntax:** `div+p`  
**Output:** `<div></div><p></p>`

**Example:**
```html
h1+h2 → <h1></h1><h2></h2>
```

### 4. Element Multiplication

Create multiple elements at once using the multiplication operator `*`.

**Syntax:** `ul>li*3`  
**Output:** 
```html
<ul>
  <li></li>
  <li></li>
  <li></li>
</ul>
```

**Example:**
```html
p*2 → <p></p><p></p>
```

### 5. Element with ID

Add an ID to an element using the `#` symbol.

**Syntax:** `div#header`  
**Output:** `<div id="header"></div>`

**Example:**
```html
p#intro → <p id="intro"></p>
```

### 6. Element with Class

Add a class to an element using the `.` symbol.

**Syntax:** `div.container`  
**Output:** `<div class="container"></div>`

**Example:**
```html
p.text → <p class="text"></p>
```

### 7. Multiple Classes

Add multiple classes to an element by chaining `.` symbols.

**Syntax:** `div.container.flex`  
**Output:** `<div class="container flex"></div>`

**Example:**
```html
p.text.bold → <p class="text bold"></p>
```

### 8. Element with Attributes

Add custom attributes to elements using square brackets.

**Syntax:** `a[href=#]`  
**Output:** `<a href="#"></a>`

**Example:**
```html
img[src=image.jpg] → <img src="image.jpg">
```

### 9. Element with Text

Add text content to an element using curly braces.

**Syntax:** `p{Hello}`  
**Output:** `<p>Hello</p>`

**Example:**
```html
h1{Title} → <h1>Title</h1>
```

### 10. Grouping

Group elements together using parentheses to create complex structures.

**Syntax:** `div>(header>ul>li*2)+footer`  
**Output:** 
```html
<div>
  <header>
    <ul>
      <li></li>
      <li></li>
    </ul>
  </header>
  <footer></footer>
</div>
```

**Example:**
```html
(div>p)+div → <div><p></p></div><div></div>
```

![HTML Basics](https://unsplash.com/photos/xkBaqlcqeb4/download?ixid=M3wxMjA3fDB8MXxzZWFyY2h8M3x8aHRtbHxlbnwwfHx8fDE3MTYxNDcyMzl8MA&force=true&w=1920)

## Advanced HTML Techniques

### 11. Numbering

Use the `$` symbol to automatically number elements.

**Syntax:** `ul>li.item$*3`  
**Output:** 
```html
<ul>
  <li class="item1"></li>
  <li class="item2"></li>
  <li class="item3"></li>
</ul>
```

**Example:**
```html
h$*3 → <h1></h1><h2></h2><h3></h3>
```

### 12. Custom Numbering Base

Start numbering from a specific number using `$@n`.

**Syntax:** `ul>li.item$@3*3`  
**Output:** 
```html
<ul>
  <li class="item3"></li>
  <li class="item4"></li>
  <li class="item5"></li>
</ul>
```

**Example:**
```html
p.item$@5*3 → <p class="item5"></p><p class="item6"></p><p class="item7"></p>
```

### 13. Reverse Numbering

Reverse the numbering order using `$@-`.

**Syntax:** `ul>li.item$@-*3`  
**Output:** 
```html
<ul>
  <li class="item3"></li>
  <li class="item2"></li>
  <li class="item1"></li>
</ul>
```

**Example:**
```html
h$@-*3 → <h3></h3><h2></h2><h1></h1>
```

### 14. Numbering with Text

Combine numbering with text content.

**Syntax:** `ul>li.item${Item $}*3`  
**Output:** 
```html
<ul>
  <li class="item1">Item 1</li>
  <li class="item2">Item 2</li>
  <li class="item3">Item 3</li>
</ul>
```

**Example:**
```html
p{Paragraph $}*2 → <p>Paragraph 1</p><p>Paragraph 2</p>
```

### 15. Lorem Ipsum Generator

Generate Lorem Ipsum placeholder text.

**Syntax:** `p>lorem`  
**Output:** `<p>Lorem ipsum dolor sit amet...</p>`

**Example:**
```html
p>lorem10 → <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eos, debitis.</p>
```

### 16. Implicit Tag Names

Omit tag names to use the default tag (usually div for most cases).

**Syntax:** `.container`  
**Output:** `<div class="container"></div>`

**Example:**
```html
#header → <div id="header"></div>
```

### 17. Form Elements

Use abbreviations for common form elements and attributes.

**Syntax:** `form:post`  
**Output:** `<form action="" method="post"></form>`

**Example:**
```html
input:email → <input type="email" name="email" id="email">
```

### 18. HTML5 Doctype

Generate an HTML5 document structure with a single character.

**Syntax:** `!`  
**Output:** (full HTML5 document structure)

### 19. Meta Tags

Use abbreviations for common meta tags.

**Syntax:** `meta:vp`  
**Output:** `<meta name="viewport" content="width=device-width, initial-scale=1.0">`

**Example:**
```html
meta:utf → <meta http-equiv="Content-Type" content="text/html;charset=UTF-8">
```

### 20. Link Tags

Use abbreviations for common link elements.

**Syntax:** `link:css`  
**Output:** `<link rel="stylesheet" href="style.css">`

**Example:**
```html
link:favicon → <link rel="shortcut icon" type="image/x-icon" href="favicon.ico">
```

![Advanced HTML](https://unsplash.com/photos/UYsBCu9RP3Y/download?ixid=M3wxMjA3fDB8MXxzZWFyY2h8Nnx8aHRtbHxlbnwwfHx8fDE3MTYxNDcyMzl8MA&force=true&w=1920)

## CSS Techniques

### 21. CSS Properties

Use abbreviations for common CSS properties.

**Syntax:** `m10`  
**Output:** `margin: 10px;`

**Example:**
```css
p20 → padding: 20px;
```

### 22. Multiple Values

Specify multiple values for CSS properties.

**Syntax:** `m10-20`  
**Output:** `margin: 10px 20px;`

**Example:**
```css
p10-20-30 → padding: 10px 20px 30px;
```

### 23. Color Values

Use shortcuts for color values.

**Syntax:** `c#3`  
**Output:** `color: #333;`

**Example:**
```css
bgc#f → background-color: #fff;
```

### 24. Vendor Prefixes

Add vendor prefixes to CSS properties.

**Syntax:** `-bdrs10`  
**Output:** 
```css
-webkit-border-radius: 10px;
-moz-border-radius: 10px;
border-radius: 10px;
```

**Example:**
```css
-trf → -webkit-transform: ; -moz-transform: ; -ms-transform: ; -o-transform: ; transform: ;
```

### 25. Value Units

Specify units for CSS values.

**Syntax:** `w100p`  
**Output:** `width: 100%;`

**Example:**
```css
h50e → height: 50em;
```

### 26. Important Flag

Add the !important flag to CSS properties.

**Syntax:** `c#f!`  
**Output:** `color: #fff !important;`

**Example:**
```css
m0! → margin: 0 !important;
```

### 27. Gradients

Create CSS gradients.

**Syntax:** `lg(to right, #f00, #ff0)`  
**Output:** `background-image: linear-gradient(to right, #f00, #ff0);`

**Example:**
```css
lg(45deg, #f00, #ff0) → background-image: linear-gradient(45deg, #f00, #ff0);
```

### 28. Positioning

Use abbreviations for positioning properties.

**Syntax:** `pos:a`  
**Output:** `position: absolute;`

**Example:**
```css
pos:r → position: relative;
```

### 29. Display Properties

Use abbreviations for display properties.

**Syntax:** `d:f`  
**Output:** `display: flex;`

**Example:**
```css
d:g → display: grid;
```

### 30. Text Properties

Use abbreviations for text properties.

**Syntax:** `ta:c`  
**Output:** `text-align: center;`

**Example:**
```css
fw:b → font-weight: bold;
```

![CSS Techniques](https://unsplash.com/photos/5fNmWej4tAA/download?ixid=M3wxMjA3fDB8MXxzZWFyY2h8Mnx8Y3NzfGVufDB8fHx8MTcxNjE0NzI3OXww&force=true&w=1920)

## Workflow Optimization

### 31. Wrap with Abbreviation

Wrap selected content with an Emmet abbreviation.

**Example:** Select text → Wrap with `ul>li` → `<ul><li>selected text</li></ul>`

### 32. Balance Tag

Select the content between opening and closing tags.

**Example:** Place cursor inside tag → Balance → Selects content between tags

### 33. Go to Matching Pair

Jump between opening and closing tags.

**Example:** Place cursor at opening tag → Go to Matching Pair → Jumps to closing tag

### 34. Remove Tag

Remove the tag but keep its content.

**Example:** `<div>content</div>` → Remove Tag → `content`

### 35. Split/Join Tag

Split a tag into opening and closing tags or join them.

**Example:** `<div/>` → Split/Join Tag → `<div></div>`

### 36. Comment Section

Wrap selection with comment tags.

**Example:** Select code → Comment → `<!-- code -->`

### 37. Evaluate Math Expression

Calculate mathematical expressions within the editor.

**Example:** Select `2+4` → Evaluate Math → `6`

### 38. Increment/Decrement Number

Increase or decrease numeric values.

**Example:** Select `5` → Increment → `6`

### 39. Update Image Size

Automatically update width and height attributes of an image.

**Example:** `<img src="image.jpg">` → Update Image Size → `<img src="image.jpg" width="100" height="100">`

### 40. Encode/Decode Image to Data URL

Convert images to data URLs and vice versa.

**Example:** `<img src="image.jpg">` → Encode → `<img src="data:image/jpeg;base64,...">`

![Workflow Optimization](https://unsplash.com/photos/FGXqbqbGt5o/download?ixid=M3wxMjA3fDB8MXxzZWFyY2h8MTB8fHdvcmtmbG93fGVufDB8fHx8MTcxNjE0NzMwNnww&force=true&w=1920)

## Framework-Specific Techniques

### 41. React Components

Create React components with className instead of class.

**Syntax:** `Div.container>h1{Title}+p{Content}`  
**Output:** `<Div className="container"><h1>Title</h1><p>Content</p></Div>`

**Example:**
```jsx
Input[type=text] → <Input type="text" />
```

### 42. Vue Directives

Add Vue.js directives to elements.

**Syntax:** `div[v-for="item in items"]`  
**Output:** `<div v-for="item in items"></div>`

**Example:**
```html
input[v-model=name] → <input v-model="name">
```

### 43. Angular Directives

Add Angular directives to elements.

**Syntax:** `div[*ngFor="let item of items"]`  
**Output:** `<div *ngFor="let item of items"></div>`

**Example:**
```html
input[(ngModel)=name] → <input [(ngModel)]="name">
```

### 44. JSX Fragments

Create React fragments in JSX.

**Syntax:** `<>`  
**Output:** `<></>`

**Example:**
```jsx
<>div+div</> → <><div></div><div></div></>
```

### 45. Svelte Directives

Add Svelte directives to elements.

**Syntax:** `div[#if={condition}]`  
**Output:** `<div #if={condition}></div>`

**Example:**
```html
input[bind:value={name}] → <input bind:value={name}>
```

![Framework-Specific](https://unsplash.com/photos/m_HRfLhgABo/download?ixid=M3wxMjA3fDB8MXxzZWFyY2h8Mnx8cmVhY3R8ZW58MHx8fHwxNzE2MTQ3MzI5fDA&force=true&w=1920)

## Custom Configurations

### 46. Custom Snippets

Create your own custom Emmet snippets for frequently used code patterns.

**Example:** Define 'ui-card' → `<div class="card"><div class="card-header"></div><div class="card-body"></div></div>`

### 47. Extend Emmet

Extend Emmet's functionality with custom actions and filters.

**Example:** Create custom action to generate specific code patterns

### 48. Editor Integration

Configure Emmet to work with different editors and customize keyboard shortcuts.

**Example:** Set up custom keybindings for Emmet actions in VS Code

### 49. Emmet Preferences

Customize Emmet's behavior through preferences.

**Example:** Configure output format, indentation, BEM support, etc.

### 50. Emmet in Non-HTML Contexts

Use Emmet in JSX, XML, Haml, Pug, and other markup languages.

**Example:** Configure Emmet to work with different syntax formats

![Custom Configurations](https://unsplash.com/photos/iar-afB0QQw/download?ixid=M3wxMjA3fDB8MXxzZWFyY2h8Mnx8Y29uZmlndXJhdGlvbnxlbnwwfHx8fDE3MTYxNDczNTB8MA&force=true&w=1920)

## Resources and Further Learning

### Official Documentation

- [Emmet Documentation](https://docs.emmet.io/)
- [Emmet Cheat Sheet](https://docs.emmet.io/cheat-sheet/)

### Editor-Specific Guides

- [Emmet in Visual Studio Code](https://code.visualstudio.com/docs/editor/emmet)
- [Emmet in Sublime Text](https://packagecontrol.io/packages/Emmet)
- [Emmet in WebStorm](https://www.jetbrains.com/help/webstorm/emmet.html)

### Video Tutorials

- [Emmet in 15 Minutes](https://www.youtube.com/watch?v=V8vizNQKtx0)
- [Advanced Emmet Techniques](https://www.youtube.com/watch?v=5BIAdWNcr8Y)



