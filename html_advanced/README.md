# HTML Basics: Structuring Web Content

- [HTML Basics: Structuring Web Content](#html-basics-structuring-web-content)
  - [Glossary (in alphabetical order)](#glossary-in-alphabetical-order)
  - [What is HTML?](#what-is-html)
    - [Basic Syntax](#basic-syntax)
  - [HTML5 Page Skeleton](#html5-page-skeleton)
  - [Semantic HTML Tags](#semantic-html-tags)
  - [Div vs Span](#div-vs-span)
  - [Headings](#headings)
  - [Lists in HTML](#lists-in-html)
  - [Media Types](#media-types)
  - [Tables](#tables)
  - [Embedding Media](#embedding-media)
    - [Video](#video)
    - [Audio](#audio)
  - [Embedding External Content](#embedding-external-content)
  - [HTML Best Practices and Guidelines](#html-best-practices-and-guidelines)
  - [Author](#author)


## Glossary (in alphabetical order)

**A**
- **Attribute:** Additional information provided within HTML tags to modify the behavior or display of elements.

**B**
- **Block-level element:** An HTML element that typically starts on a new line and takes up the full width available.

**C**
- **CSS (Cascading Style Sheets):** A style sheet language used for describing the presentation of a document written in HTML.

**D**
- **DOM (Document Object Model):** A programming interface for HTML and XML documents, representing the structure of a document as a tree-like hierarchy.

**E**
- **Element:** The basic building block of HTML, consisting of a start tag, content, and an end tag.

**F**
- **Form:** An HTML element used to collect user input and submit data to a server.

**G**
- **GIF (Graphics Interchange Format):** An image file format that supports both static and animated images.

**H**
- **HTML (Hypertext Markup Language):** The standard markup language for creating web pages and web applications.

**I**
- **Inline element:** An HTML element that does not start on a new line and only takes up as much width as necessary.

**J**
- **JPG/JPEG (Joint Photographic Experts Group):** A commonly used image format for photographs and complex images.

**L**
- **Link:** An HTML element that creates a hyperlink to another web page or resource.

**M**
- **Metadata:** Information about the HTML document, typically placed within the <head> element.

**N**
- **Nesting:** The practice of placing one HTML element inside another element.

**P**
- **PNG (Portable Network Graphics):** An image format that supports transparency and is ideal for graphics with text or sharp edges.

**S**
- **Semantic HTML:** The use of HTML markup to reinforce the meaning of the content, rather than just to define its appearance.
- **SVG (Scalable Vector Graphics):** An XML-based vector image format for two-dimensional graphics.

**T**
- **Tag:** The markup syntax used to define HTML elements, enclosed in angle brackets.

**V**
- **Validation:** The process of checking HTML code for compliance with web standards and best practices.

## What is HTML?

**Definition**
HTML (Hypertext Markup Language) is the standard markup language for creating web pages. It describes the structure of a web page using a series of elements represented by tags.

### Basic Syntax

HTML uses tags to define elements. Tags are enclosed in angle brackets, and most elements have an opening and a closing tag.

*Example:*

```html
<tagname>Content goes here</tagname>
```

**Explanations:**
- **`<tagname>`**: Opening tag
- **`</tagname>`**: Closing tag
- Content is placed between the opening and closing tags

## HTML5 Page Skeleton

The basic structure of an HTML5 page includes several key elements:

*Example:*

```html
<!DOCTYPE html>
<html dir="ltr" lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Web Page</title>
</head>
<body>
    <!-- Content goes here -->
</body>
</html>
```

**Explanations:**
- **`<!DOCTYPE html>`**: Declares that this is an HTML5 document
- **`<html>`**: The root element of the HTML page
  - *`dir="ltr"`:* Indicate direction of reading, `ltr` for left to right and `rtl` for right to left.
  - *`lang=en`:* Indicate language used
- **`<head>`**: Contains meta information about the document
- **`<body>`**: Contains the visible page content

## Semantic HTML Tags

Semantic HTML tags provide meaning to the structure of web content. They help both browsers and developers understand the purpose of different parts of a web page.

*Example:*

```html
<header>
    <nav>
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
        </ul>
    </nav>
</header>
<main>
    <article>
        <h1>Welcome to My Website</h1>
        <p>This is the main content of the page.</p>
    </article>
    <aside>
        <h2>Related Links</h2>
        <ul>
            <li><a href="#link1">Link 1</a></li>
            <li><a href="#link2">Link 2</a></li>
        </ul>
    </aside>
</main>
<footer>
    <p>&copy; 2023 My Website</p>
</footer>
```

**Explanations:**
- **`<header>`**: Represents introductory content or a group of navigational aids
- **`<nav>`**: Defines a section of navigation links
- **`<main>`**: Specifies the main content of the document
- **`<article>`**: Represents a self-contained composition in a document
- **`<aside>`**: Defines content aside from the main content (like a sidebar)
- **`<footer>`**: Represents a footer for a document or section

## Div vs Span

- **`<div>`**: A block-level container for grouping elements
- **`<span>`**: An inline container for phrasing content

Use cases:
- Use **`<div>`** for larger sections of content or layout purposes
- Use **`<span>`** for small portions of text or inline elements

*Example:*

```html
<div class="container">
    <p>This is a paragraph with <span class="highlight">highlighted</span> text.</p>
</div>
```

## Headings

HTML provides six levels of headings, from `<h1>` to `<h6>`. It's important to follow the hierarchical order for proper document structure and SEO.

*Example:*

```html
<h1>Main Title</h1>
<h2>Subtitle</h2>
<h3>Section Heading</h3>
<h4>Subsection Heading</h4>
```

**Why it's important:**
- Improves accessibility for screen readers
- Helps search engines understand the content structure
- Creates a clear visual hierarchy for users

## Lists in HTML

HTML supports three types of lists:

1. Unordered lists (`<ul>`)
2. Ordered lists (`<ol>`)
3. Description lists (`<dl>`)

*Example:*

```html
<ul>
    <li>Unordered item 1</li>
    <li>Unordered item 2</li>
</ul>

<ol>
    <li>Ordered item 1</li>
    <li>Ordered item 2</li>
</ol>

<dl>
    <dt>Term 1</dt>
    <dd>Description 1</dd>
    <dt>Term 2</dt>
    <dd>Description 2</dd>
</dl>
```

## Media Types

Different media types have various use cases:

- **SVG**: Scalable Vector Graphics, ideal for logos and icons
- **GIF**: Supports animations, good for simple animated images
- **PNG**: Supports transparency, best for images with text or sharp edges
- **JPG**: Best for photographs and complex images with many colors

## Tables

Tables are used to structure data in rows and columns.

*Example:*

```html
<table>
    <thead>
        <tr>
            <th>Header 1</th>
            <th>Header 2</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Row 1, Cell 1</td>
            <td>Row 1, Cell 2</td>
        </tr>
        <tr>
            <td>Row 2, Cell 1</td>
            <td>Row 2, Cell 2</td>
        </tr>
    </tbody>
</table>
```

**Explanations:**
- **`<table>`**: Defines an HTML table, which is used to organize data in a grid-like structure with rows and columns.
- **`<thead>`**: This element groups the header content of the table, typically containing the column names or titles.
- **`<tr>`**: Represents a table row, which can contain one or more table cells (`<th>` or `<td>`).
- **`<th>`**: Defines a table header cell, typically used for column headers. The content within `<th>` elements is often rendered in bold by default.
- **`<tbody>`**: This element groups the body content of the table, containing the actual data rows.
- **`<td>`**: Defines a table data cell, which contains the data for a specific row and column intersection.

In this example, the table has a header row with two column headers ("Header 1" and "Header 2"), and two data rows, each with two data cells. The `<thead>` and `<tbody>` elements help to semantically structure the table content, making it easier for browsers and screen readers to understand the organization of the data.

## Embedding Media

### Video

Use the `<video>` tag to embed videos in a webpage.

*Example:*

```html
<video width="320" height="240" controls>
    <source src="movie.mp4" type="video/mp4">
    Your browser does not support the video tag.
</video>
```

### Audio

Use the `<audio>` tag to embed audio files.

*Example:*

```html
<audio controls>
    <source src="audio.mp3" type="audio/mpeg">
    Your browser does not support the audio element.
</audio>
```

## Embedding External Content

Use the `<iframe>` tag to embed external content like maps or videos from other websites.

*Example:*

```html
<iframe src="https://www.youtube.com/embed/dQw4w9WgXcQ" width="560" height="315" frameborder="0" allowfullscreen></iframe>
```

## HTML Best Practices and Guidelines

1. Use semantic HTML tags appropriately
2. Maintain a clear document structure
3. Use descriptive and meaningful tag and attribute names
4. Ensure proper nesting of elements
5. Validate your HTML code
6. Use comments to explain complex structures
7. Keep your code clean and well-formatted
8. Use lowercase for tag names and attributes
9. Always close your tags
10. Use the lang attribute on the `<html>` tag

## Author

Arc + NotDiamond(AI)