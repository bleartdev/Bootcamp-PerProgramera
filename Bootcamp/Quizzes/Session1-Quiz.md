# HTML Basics — Session 1 Overview

A concise overview of the core concepts of **HTML (HyperText Markup Language)**.

---

## Table of Contents

1. [What is HTML?](#1-what-is-html)
2. [Types of tags](#2-types-of-tags)
3. [HTML document structure](#3-html-document-structure)
4. [What goes inside `<head>`](#4-what-goes-inside-head)
5. [What goes inside `<body>`](#5-what-goes-inside-body)
6. [How elements are rendered](#6-how-elements-are-rendered)
7. [Block vs Inline elements](#7-block-vs-inline-elements)
8. [Comments in HTML](#8-comments-in-html)
9. [Text formatting tags](#9-text-formatting-tags)
10. [Semantic HTML tags](#10-semantic-html-tags)
11. [Semantic vs non-semantic tags](#11-semantic-vs-non-semantic-tags)
12. [Four semantic tags](#12-four-semantic-tags)
13. [Types of lists](#13-types-of-lists)
14. [Tags for each list type](#14-tags-for-each-list-type)
15. [Links and attributes](#15-links-and-attributes)
16. [Types of links](#16-types-of-links)
17. [`img` vs `figure`](#17-img-vs-figure)
18. [Tags for images and figures](#18-tags-for-images-and-figures)

---

## 1. What is HTML?

HTML is a markup language used to build the **structure of web pages**.  
It is not a programming language. HTML tells the browser how content
should be organized and displayed.

---

## 2. Types of tags

HTML tags are used to define and structure content on a web page.
They can be divided into two main categories.

### 2.1 Opening and closing tags
These tags consist of an opening tag and a closing tag and wrap content
between them.

```html

<p>Text</p>

```

### 2.2 Self-closing tags

These tags do not require a closing tag and are used for elements
that do not contain content.

```html
<img />
<br />
<hr />
```
---
## 3. HTML document structure

Every HTML document follows a basic structure that tells the browser
how to interpret and render the page content.

```html
<!DOCTYPE html>
<html>
  <head>
    <!-- Meta tags, title, CSS -->
  </head>
  <body>
    <!-- Visible page content -->
  </body>
</html>
```
- `<!DOCTYPE html>` declares the document as HTML5
- `<html>` is the root element of the document
- `<head>` contains metadata and configuration information
- `<body>` contains the content displayed in the browser

---
## 4. What goes inside `<head>`?

The `<head>` section of an HTML document contains information that is
**not displayed directly** on the web page but is essential for the
browser and search engines.

Common elements placed inside `<head>` include:

- `<meta>` — defines character encoding, viewport, description, keywords
- `<title>` — the page title shown in the browser tab
- `<link>` — used to connect external stylesheets (CSS)
- Metadata for SEO and site identity (favicon, etc.)


---

## 5. What goes inside `<body>`?

The `<body>` section contains the **visible content** of a web page,
which is rendered directly in the browser.

Elements commonly placed inside `<body>` include:

- Text (headings, paragraphs, quotes)
- Images (`<img>`)
- Links (`<a>`)
- Lists (`<ul>`, `<ol>`)
- Tables (`<table>`)
- Forms (`<form>`)

---

## 6. How elements are rendered

In HTML, elements are rendered by the browser based on how they are defined.
Most elements fall into one of two categories:

- **Block elements**
- **Inline elements**

This distinction affects how elements are positioned and displayed
in relation to other content on the page.


---

## 7. Block vs Inline elements

HTML elements behave differently depending on how they are rendered.

### Block elements
- Occupy the full width of the line
- Always start on a new line
- Can contain other elements

Common examples:
`<div>`, `<p>`, `<h1>` – `<h6>`, `<section>`

### Inline elements
- Occupy only the space of their content
- Do not start on a new line
- Appear within the flow of text

Common examples:
`<span>`, `<a>`, `<strong>`, `<em>`

---

## 8. Comments in HTML

Comments in HTML are used for **explanation, documentation, and maintenance**
of code without being displayed on the web page.

They help developers understand the structure and logic of the code,
especially in larger projects.

Browsers **do not render comments**.

```html

<!-- This is an HTML comment -->

```

---

## 9. Text formatting tags

HTML uses different tags to **format and structure text** on a web page.
These tags help highlight content and improve readability.

Commonly used text formatting tags include:

- **Bold:** `<b>`, `<strong>`
- **Italic:** `<i>`, `<em>`
- **Underline:** `<u>`
- **Subscript / Superscript:** `<sub>`, `<sup>`
- **Headings:** `<h1>` to `<h6>`

---

## 10. Semantic HTML tags

Semantic HTML tags are elements that clearly describe the **meaning and role**
of the content they contain.

They help:
- Browsers and search engines (SEO)
- Accessibility tools
- Developers understand the structure of a page

Examples of semantic HTML tags:
`<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`

---

## 11. Semantic vs non-semantic tags

In HTML, there is a clear distinction between **non-semantic** and
**semantic** tags.

- **Non-semantic tags** (e.g. `<div>`, `<span>`)  
  Do not describe the meaning of their content and are mainly used
  for layout or styling purposes.

- **Semantic tags** (e.g. `<header>`, `<nav>`, `<main>`, `<footer>`)  
  Clearly define the role of the content and help improve:
  - SEO
  - Accessibility
  - Code readability

---

## 12. Four semantic tags

Some commonly used semantic HTML tags include:

- `<header>` — represents the top section of a page (logo, title, navigation)
- `<nav>` — contains the main navigation links
- `<main>` — represents the main content of the page
- `<footer>` — represents the bottom section (copyright, links)


---

## 13. Types of lists

HTML supports three main types of lists, which are used to organize
content in a structured way.

- **Ordered list** — a numbered list
- **Unordered list** — a bulleted list
- **Description list** — a list of terms and their descriptions

---

## 14. Tags for each list type

Each list type in HTML uses specific tags:

- **Ordered list:** `<ol>` and `<li>`
- **Unordered list:** `<ul>` and `<li>`
- **Description list:** `<dl>`, `<dt>`, and `<dd>`


---

## 15. Links and attributes

The `<a>` tag is used to create links in HTML.

Common attributes of the `<a>` tag include:
- **`href`** — specifies the destination URL
- **`target`** — defines where the link opens (e.g. `_blank`)
- **`title`** — adds additional information displayed as a tooltip

Example:
```html

<a href="https://example.com" target="_blank" title="Example">Example</a>

```

----

## 16. Types of links

In HTML, links are used to navigate between pages and resources.
They are generally categorized into two main types:

- **Internal links**  
  Used to link pages within the same website or project.

- **External links**  
  Used to link to pages or resources outside the current website.

---

## 17. `img` vs `figure`

There is an important difference between the `<img>` and `<figure>` tags in HTML.

- **`<img>`**  
  Displays only the image itself and is typically used for decorative
  or standalone images.

- **`<figure>`**  
  Wraps an image together with a caption using `<figcaption>`,
  and is commonly used when the image has contextual meaning.


## 18. Tags for images and figures

To work with images and figures in HTML, the following tags are used:

- **`<img>`** — displays an image on the page
- **`<figure>`** — groups an image with related content
- **`<figcaption>`** — provides a caption or description for the image

Example:
```html
<figure>
  <img src="photo.jpg" alt="Sample image">
  <figcaption>Image description</figcaption>
</figure>
```