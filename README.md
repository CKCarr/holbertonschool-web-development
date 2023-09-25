# css_advanced
### Learning Objectives

## Table of Contents
[CLICK HERE! to launch HTML/CSS Advanced website link](https://ckcarr.github.io/holbertonschool-web-development/)
1. [What is CSS](#what-is-css)
2. [How to Add Style to an Element](#how-to-add-style-to-an-element)
3. [What is a Class](#what-is-a-class)
4. [What is a Selector](#what-is-a-selector)
5. [How to Compute CSS Specificity Value](#how-to-compute-css-specificity-value)
6. [What are Box Properties in CSS](#what-are-box-properties-in-css)
7. [How Does the Browser Load a Webpage](#how-does-the-browser-load-a-webpage)

![Header and Banner](images/header%20and%20banner.jpg)

<h3>What is CSS</h3>

CSS stands for Cascading Style Sheets. It is a stylesheet language used to describe how HTML elements should look on a webpage.<br>
HTML structures the content, CSS styles it. You can change font sizes, colors, add margins, and much more using CSS. It is important because CSS makes web pages visually appealing as well as
separating content (HTML) from styling (CSS), making it easier to maintain.


<h3>How to add style to an element</h3>

1. <b>Inline Style:</b> Directly within the HTML element using the 'style' attribute.
```
<p style="color: red;">This is red text.</p>
```
2. <b>Internal Style Sheet:</b> Within the HTML file but inside the \<head> section using \<style> tags.
```
<style>
  p {
    color: red;
  }
</style>
```
3. <b>External Style Sheet:</b> In a separate .css file, linked to the HTML file.
```
/* styles.css */
p {
  color: red;
}
```
```
<!-- index.html -->
<link rel="stylesheet" href="styles.css">
```
- <b>Best Practices</b><br>
Use external stylesheets for larger projects for better organization and reusability.


<h3>What is a class</h3>

In CSS, a class is a way to select multiple elements that share the same styling. Unlike IDs, which are unique, classes can be reused. This allows you to apply the same style to multiple elements without repeating code.
```
.my-class {
  font-size: 20px;
  color: blue;
}
```
<h3>What is a selector</h3>

A selector in CSS is used to target HTML elements and apply styles to them. They are the building blocks of CSS, allowing you to target what you want to style.<br>
<b>Types of selectors include:</b>

- <b>Type selectors:</b> Target by element type (p, h1)
- <b>Class selectors:</b> Target by class (.my-class)
- <b>ID selectors:</b> Target by ID (#my-id)


<h3>How to compute CSS Specificity Value</h3>

The specificity of a CSS rule is determined by a set of rules usually calculated in a (0,0,0,0) format:

- !Important flagged styles.<br>([#]-0-0-0-0)
- Inline styles: Highest specificity.<br>([#]-0-0-0)
- IDs: More specific than any class.<br>([#]-0-0)
- Classes, attributes, and pseudo-classes: Next level down.<br>(0-[#]-0)
- Type selectors and pseudo-elements: Lowest level.<br>(0-0-[#])

EXAMPLES:
- ' .my-class p ': (0,1,1) - 0 IDs, 1 Class, 1 Element
- ' #my-id .my-class ': (1,1,0) - 1 ID, 1 Class, 0 Elements

<section>
<h3>What are Box properties in CSS</h3>

These properties help in arranging elements properly on a page.
These properties control layout:
- <b>Margin:</b> Outside the border.
- <b>Border:</b> Surrounds the padding and content.
- <b>Padding:</b>  Inside the border, outside the content.
- <b>Content:</b> The actual content.
<img src="images/CSS-Box-Model.webp" alt="box-model-css" width="300"/>
</section>

<section>
<h3>How does the browser load a webpage</h3><br>

1. <b>DNS Lookup:</b> Translates URL to IP address.
- The browser converts the human-friendly URL into an IP address.
2. <b>HTTP Request:</b> Browser requests data.
- The browser asks the server at that IP address for the webpage content.
3. <b>Server Response:</b> Sends back files.
- The server sends back the necessary files like HTML, CSS, and JS.
4. <b>Browser Render:</b> Parses HTML and CSS, runs JS, and renders the page.
- Finally, your browser combines these files to display the webpage you see.
</section>
