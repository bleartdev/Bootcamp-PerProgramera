# HTML Basics — Session 2 Overview

An overview of more advanced **HTML elements** related to images, maps, tables, meta tags, and forms.

---

## Table of Contents

1. [What are responsive images and through which HTML tag are they implemented?](#1-what-are-responsive-images-and-through-which-html-tag-are-they-implemented)
2. [What are image maps and what is their benefit in HTML?](#2-what-are-image-maps-and-what-is-their-benefit-in-html)
3. [How many types of image maps are there?](#3-how-many-types-of-image-maps-are-there)
4. [What are meta tags and what are they used for?](#4-what-are-meta-tags-and-what-are-they-used-for)
5. [What is the mechanism for creating tables and structuring rows and columns?](#5-what-is-the-mechanism-for-creating-tables-and-structuring-rows-and-columns)
6. [Which attributes can be used in tables?](#6-which-attributes-can-be-used-in-tables)
7. [How is a long table structured in HTML?](#7-how-is-a-long-table-structured-in-html)
8. [Name 12 input types used in HTML web forms](#8-name-12-input-types-used-in-html-web-forms)

---

## 1. What are responsive images and through which HTML tag are they implemented?

Responsive images are images that **adapt automatically** to different screen sizes such as mobile phones, tablets, and desktop devices.

They are mainly implemented using the `<picture>` tag together with `<source>` and `<img>`.

```html
<picture>
  <source media="(max-width: 600px)" srcset="mobile.jpg">
  <source media="(min-width: 601px)" srcset="desktop.jpg">
  <img src="default.jpg" alt="Responsive image">
</picture>
```

---

## 2. What are image maps and what is their benefit in HTML?

Image maps are images that contain **clickable areas**, where each area can link to a different page or resource.

Their main benefit is that they allow **interaction with specific parts of an image**, enabling multiple links within a single image.

---

## 3. How many types of image maps are there?

There are **three types** of clickable areas used in HTML image maps:
- `rect` — rectangle
- `circle` — circle
- `poly` — polygon (custom shape)
---
## 4. What are meta tags and what are they used for?

Meta tags are HTML elements placed inside the `<head>` section of a document.

They are used to:
- Define character encoding
- Control responsive behavior
- Improve SEO
- Provide information about the web page
---
## 5. What is the mechanism for creating tables and structuring rows and columns?

Tables in HTML are created using the following tags:
- `<table>` — table container
- `<tr>` — table row
- `<th>` — table header cell
- `<td>` — table data cell
---

## 6. Which attributes can be used in tables?

Some commonly used table-related attributes include:
- `colspan`
- `rowspan`
- `border`
- `cellspacing`
- `cellpadding`
- `class`, `id`, `style`
---
## 7. How is a long table structured in HTML?

When a table contains a large amount of data, it is structured using:
- `<thead>` — table header
- `<tbody>` — table body
- `<tfoot>` — table footer
---
## 8. Name 12 input types used in HTML web forms

Commonly used HTML input types include:
- `text`
- `password`
- `email`
- `number`
- `tel`
- `url`
- `date`
- `time`
- `checkbox`
- `radio`
- `file`
- `submit`
### Example

```html
<form>
  <input type="text" placeholder="Full Name">
  <input type="email" placeholder="Email">
  <input type="password" placeholder="Password">
  <input type="submit" value="Submit">
</form>
```


