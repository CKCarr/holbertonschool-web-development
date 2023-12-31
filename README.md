# holbertonschool-web-development


[CLICK HERE! to launch HTML/CSS Advanced website link](https://ckcarr.github.io/holbertonschool-web-development/)


# HTML_Advanced

<details open><summary>What is HTML</summary>
HTML stands for HyperText Markup Language. It's the standard markup language used to create web pages. HTML provides the structure for the content that appears on web browsers. Think of it like the "skeleton" of a web page, providing a place for other technologies like CSS (styling) and JavaScript (interactivity) to attach to.
</details>
<br>
<details open><summary>How to create an HTML page from a wireframe</summary>
 Look at your wireframe and identify the elements you'll need (headers, paragraphs, links, images, etc.).
 <br>
 
Create HTML Skeleton:
 Start with the basic HTML structure
  (\<!DOCTYPE html>, \<html>, \<head>, \<body>).

Add Semantic Elements:
Use HTML tags that correspond to the elements you identified in your wireframe. Add them within the \<body> of your HTML document.

Annotate with Comments:
If your WireFrame is complex, you might add HTML comments (\<!-- like this -->) to describe what each section is for.

Fill in Attributes:
Where needed, add attributes to your elements. For example, you'll need href attributes for links and src attributes for images.

Review and Test:
Double-check your code against your WireFrame. Make sure each part of the WireFrame is represented in your HTML structure.

</details>
<br>
<details open ><summary>What is a markup language</summary>
A markup language is a system for annotating a document in a way that is syntactically distinguishable from the text. In simpler terms, it's a way to describe and structure your content. For example, in HTML, you use tags like &ltp&gt for paragraphs and &lth1&gt for a level-one header.
</details>
<br>
<details open><summary>What is the DOM</summary>
DOM stands for Document Object Model. It's a programming interface that allows you to interact with HTML (and XML) documents programmatically. When a web page is loaded, the browser creates the DOM of the page, which is an object-oriented representation of the web page's structure.
</details>
<br>
<details open><summary>What is an element / tag</summary>
An element or tag in HTML defines the structure and content in an HTML document. Elements are written with a start tag, some content, and an end tag. For example, a paragraph is created using the &ltp&gt (start tag), some text, and &lt/p&gt (end tag).
</details>
<br>
<details open><summary>What is an attribute</summary>
Attributes provide additional information about an element. They're placed within the opening tag. For example, in &ltimg src="image.jpg" alt="An image"&gt&ltimg src="image.jpg" alt="An image"&gt, src and alt are attributes that specify the image source and alternative text, respectively.
</details>
<br>
<details open><summary>What the purpose of each HTML tag</summary>
Each tag serves a specific purpose in creating and laying out content.

```
<html>: Root element that contains all other HTML elements.
<head>: Contains meta information, links to CSS, JS files, etc.
<title>: Sets the title of the web page.
<body>: Contains the content of the web page.
<h1>, <h2>, ... <h6>: Headings to structure content.
<p>: Paragraph.
<a>: Anchor (links).
<img>: Embed images.
<ul>, <ol>, <li>: Lists.
<table>, <tr>, <td>: Table and its rows and data cells.
... and many more.
```

</details>

### WireFrame used to develop this project

![WireFrame for project](./html_advanced/HTML_advanced_wireframe.png)




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
