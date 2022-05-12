---

#Module-1
Introduction to HTML
What is HTML and Where did it come from?
HTML Syntax
Semantic
Markup
Structure of HTML Documents
Quick Tour of HTML Elements
HTML5 Semantic Structure Elements
Introduction to CSS
What is CSS
CSS Syntax
Location of Styles
Box Model
CSS Text Styling

---

Questions:
#1 Explain the role of <ul> and <ol> HTML tags with syntax and examples.

An unordered list starts with the <ul> tag. Each list item starts with the <li> tag.The list items will be marked with bullets (small black circles) by default:

example:

<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>

An ordered list starts with <ol> tag. Each list items starts with the <li> tag.The list items will be marked with numbers(1..2...3) by default.

example:

<ol>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>

---

#2 Explain the need of 'cascade' in CSS. Illustrate three principles of cascade with suitable CSS scripts segments.

CSS stands for Cascading Stylesheets. The cascade is the algorithm for solving conflicts where multiple CSS rules apply to an HTML element.

The visual metaphor behind the term cascade is that of a mountain stream progressing downstream over rocks.

The downward movement of water down a cascade is meant to be analogous to how a given style rule will continue to take precedence with child elements.

example:

button {
color: red;
}

button {
color: blue;
}

Here the color blue gets applied to the element!

Three cascade principles: INHERITENCE | SPECIFICITY | LOCATION

1. Inheritence:

Many (but not all) CSS properties affect not only themselves but their descendants as well.

Font, color, list, and text properties are inheritable.

Layout, sizing, border, background and spacing properties are not.

2. SPECIFICITY:

"an algorithm which determines which CSS selector has the strongest match"
Specificity is how the browser determines which style rule takes precedence when more than one style rule could be applied to the same element.

The more specific the selector, the more it takes precedence (i.e., overrides the previous definition)

3. Location:

When inheritance and specificity cannot determine style precedence, the principle of location will
be used.

The principle of location is that when rules have the same specificity, then the latest are given
more weight.

---

#3. Explain class selectors and pseudo selectors of CSS with relevant scripts.

A pseudo-element selector: is a way to select something that does not exist explicitly as an element in the HTML document tree but which is still a recognizable selectable object.

A pseudo-class selector does apply to an HTML element, but targets either a particular state or, in CSS3, a variety of family relationships

example:

- unvisited link \*/
  a:link {
  color: #FF0000;
  }

/_ visited link _/
a:visited {
color: #00FF00;
}

/_ mouse over link _/
a:hover {
color: #FF00FF;
}

class Selectors: A class selector allows you to simultaneously target different HTML elements regardless of their position in the document tree.

If a series of HTML element have been labelled with the same class attribute value,then you can target them for styling by using a class selector
example:

<html>
<head>

<style>
.intro {
  background-color: yellow;
}
</style>

</head>

<body>
<div class="intro">
  <p>VVCE.</p>
</div>
</body>
</html>

---

#4. Explain two types of URL referencing techniques with suitable scripts in HTML5.

Relative references:
Relative references are used when your website includes more than one page. You might choose to have several pages and a link mechanism for moving among them.

Absolute references:
Absolute references always begin with the protocol name. An absolute reference is the complete address to a web page, just as you'd use in the browser's address bar. Absolute references are used to refer to a site somewhere else on the Internet.

---

#5. Explain the role of the following semantic elements of HTML5 with syntax and script segments:

<nav>: tag defines a set of navigation links.
NOT all links of a document should be inside a <nav> element. The <nav> element is intended only for major block of navigation links.

<nav>
  <a href="/html/">HTML</a>
  <a href="/css/">CSS</a> 
  <a href="/js/">JavaScript</a>
</nav>

<section>: tag defines a section in a document.
It is used to write the document contents in a more presentable and readable sections.
.
.
.
<body>
<section>

<h2>WWF History</h2>
<p>The World Wide Fund for Nature (WWF) is an international organization working on issues regarding the conservation, research and restoration of the environment, formerly named the World Wildlife Fund. WWF was founded in 1961.</p>

</section>
</body>
.
.

<aside>: tag defines some content aside from the content it is placed in.
The aside content should be indirectly related to the surrounding content.
The <aside> content is often placed as a sidebar in a document. 
It does not render as anything special in a browser.

<aside>
<h4>some dummy heading!</h4>
<p>VVCE is an engineering college in Mysore.</p>
</aside>

---

#6. Explain following CSS property with suitable examples: FLOAT | POSITION | OVERFLOW

1. float: property specifies whether an element should float to the left, right, or not at all.
   Absolutely positioned elements ignore the float property

Elements next to a floating element will flow around it. To avoid this, use the clear property or the clearfix

Syntax:
float: none

example:
img {
float: left;
}

2. position: property specifies the type of positioning method used for an element.

There are five different position values:
static: not positioned in any special way; it is always positioned according to the normal flow of the page

relative: is positioned relative to its normal position.

fixed: is positioned relative to the viewport, which means it always stays in the same place even if the page is scrolled.

absolute: is positioned relative to the nearest positioned ancestor. Absolute positioned elements are removed from the normal flow, and can overlap elements.

sticky: is positioned based on the user's scroll position. A sticky element
toggles between relative and fixed.

3. overflow: property controls what happens to content that is too big to fit into an area
   The overflow property has the following values:

visible: The content renders outside the element's box
hidden: the rest of the content will be invisible
scroll: a scrollbar is added to see the rest of the content
auto: Similar to scroll, but it adds scrollbars only when necessary

---

#7. With Example explain HTML Syntax?

<!DOCTYPE html>
<html>
<head>
<title>Page Title</title>
</head>
<body>

<h1>First Heading</h1>
<p>first paragraph.</p>

</body>
</html>

The <!DOCTYPE html>: declaration defines that this document is an HTML5 document
The <html>: element is the root element of an HTML page
The <head>: element contains meta information about the HTML page
The <title>: element specifies a title for the HTML page (which is shown in the browser's title bar or in the page's tab)
The <body>: element defines the document's body, and is a container for all the visible contents, such as headings, paragraphs, images, hyperlinks, tables, lists, etc.
The <h1>: element defines a large heading
The <p>: element defines a paragraph

---

#8. Explain any six html elements ?

<html> </html>: All web pages start with the html element. It’s also called the root element because it’s at the root of the tree of elements that make up a web page.

<title> </title>: The title element contains the title of the page. The title is displayed in the browser’s title bar (the bar at the top of the browser window), as well as in bookmarks, search engine results, and many other places.

<h1> </h1>: Heading tags in html are used to specify a section heading!
HTML actually supports 6 heading elements->  h1, h2, h3, h4, h5, and h6. h1 is for the most important headings, h2 is for less important subheadings, and so on.

<p> </p>: Paragraph tags lets you create paragraphs of text.
Most browsers display paragraphs with a vertical gap between each paragraph, nicely breaking up the text.

<img src=" pic.jpg" alt="My picture"> : The img element lets you insert images into your web pages. You can use an <img> tag to reference an uploaded image filename.
alt attribute is required for all img tags. It’s used by browsers that don’t display images to give alternative text to the visitor.

<div> … </div>: A block-level container for content
The div element is a generic container that you can use to add more structure to your page content.You might group several paragraphs or headings that serve a similar purpose together inside a div element

************************************\_\_\_\_************************************-

#9. What is CSS? Explain the benefits of CSS.

Definition:
Cascade Style Sheet or CSS is the language we use to style an HTML document. CSS describes how HTML elements should be displayed.

The following are the advantages of CSS −

CSS saves time: − You can write CSS once and then reuse the same sheet in multiple HTML pages. You can define a style for each HTML element and apply it to as many Web pages as you want.

Easy maintenance: − To make a global change, simply change the style, and all elements in all the web pages will be updated automatically.

Global web standards: − Now HTML attributes are being deprecated and it is being recommended to use CSS. So it's a good idea to start using CSS in all the HTML pages to make them compatible with future browsers.

Platform Independence: − The Script offer consistent platform independence and can support latest browsers as well.

---

#10. With examples explain the location of styles.

-->CSS can be added to HTML documents in 3 ways

Inline: - by using the style attribute inside HTML elements
Internal: - by using a <style> element in the <head> section
External: - by using a <link> element to link to an external CSS file

---

#11. Explain two selectors with respect to CSS.
Refer question #3

---

#12. What are the three aims of HTML5 and expand the following: HTML | XML | DOCTYPE | PHP | WHATWG ?

HTML5’s three aims are

Improving the Native Web:
More Done with Less Code:
The Semantic Web:

HTML: HYPERTEXT MARKUP LANGUAGE
XML: Extensible Markup Language
PHP: HYPERTEXT PREPROCESSOR
WHATWG: Web Hypertext Application Technology Working Group

---

#13. Explain the thee types of lists in HTML5 with an example.

There are three list types in HTML:

unordered list: — used to group a set of related items in no particular order

<ul>
  <li>One</li>
  <li>Two</li>
  <li>Three</li>
</ul>

ordered list: — used to group a set of related items in a specific order

<ol>
  <li>One</li>
  <li>Two</li>
  <li>Three</li>
</ol>

description list: — used to display name/value pairs such as terms and definitions

<dl>
  <dt>Name1</dt>
  <dd>Value that applies to Name1</dd>
  <dt>Name2</dt>
  <dt>Name3</dt>
  <dd>Value that applies to both Name2 and Name3</dd>
  <dt>Name4</dt>
  <dd>One value that applies to Name4</dd>
  <dd>Another value that applies to Name4</dd>
</dl>

---
