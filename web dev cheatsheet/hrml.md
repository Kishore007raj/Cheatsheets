Here's an HTML cheatsheet following a similar format:

---

# HTML Cheatsheet and Best Practices

## Motivation
This document serves as a handy cheatsheet for developers with basic knowledge of HTML who want to brush up on essential elements, attributes, and best practices while building web pages.

**Note:** If you have basic knowledge of web development, this cheatsheet will help you structure HTML documents effectively.

---

### Table of Contents

- [HTML Structure](#html-structure)
- [Basic HTML Elements](#basic-html-elements)
- [Attributes](#attributes)
- [Head Elements](#head-elements)
- [Text Formatting](#text-formatting)
- [Links](#links)
- [Images](#images)
- [Lists](#lists)
- [Tables](#tables)
- [Forms](#forms)
- [Semantic HTML5 Elements](#semantic-html5-elements)
- [Media](#media)
- [Best Practices](#best-practices)

---

### HTML Structure

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
  </head>
  <body>
    <!-- Page content goes here -->
  </body>
</html>
```

- `<!DOCTYPE html>`: Declares the document type.
- `<html>`: Root element of the HTML document.
- `<head>`: Contains metadata and links to external files (CSS, JS).
- `<body>`: Contains all the content of the web page.

---

### Basic HTML Elements

- **Headings**: `<h1>` to `<h6>`
  
  ```html
  <h1>Main Heading</h1>
  <h2>Subheading</h2>
  ```

- **Paragraphs**: `<p>`
  
  ```html
  <p>This is a paragraph.</p>
  ```

- **Divisions**: `<div>`
  
  ```html
  <div>This is a container.</div>
  ```

- **Spans**: `<span>`
  
  ```html
  <span>Inline text container.</span>
  ```

---

### Attributes

- **Global Attributes**: `class`, `id`, `style`, `title`, `lang`, `data-*`
  
  ```html
  <div class="container" id="main-content"></div>
  ```

- **Specific Attributes**: `src`, `href`, `alt`, `target`
  
  ```html
  <img src="image.jpg" alt="Image description">
  <a href="https://example.com" target="_blank">Link</a>
  ```

---

### Head Elements

- **Meta Tags**: Defines metadata about the HTML document.
  
  ```html
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  ```

- **Title**: Sets the page title shown on browser tabs.
  
  ```html
  <title>Page Title</title>
  ```

- **Link to CSS**: Connects external CSS files.
  
  ```html
  <link rel="stylesheet" href="styles.css">
  ```

---

### Text Formatting

- **Bold**: `<b>` or `<strong>`
  
  ```html
  <b>Bold text</b>
  ```

- **Italic**: `<i>` or `<em>`
  
  ```html
  <i>Italic text</i>
  ```

- **Underline**: `<u>`
  
  ```html
  <u>Underlined text</u>
  ```

- **Line Break**: `<br>`
  
  ```html
  Text<br>New Line
  ```

- **Horizontal Rule**: `<hr>`
  
  ```html
  <hr>
  ```

---

### Links

- **Basic Link**: `<a>`
  
  ```html
  <a href="https://example.com">Visit Example</a>
  ```

- **Open in New Tab**: `target="_blank"`
  
  ```html
  <a href="https://example.com" target="_blank">Open in new tab</a>
  ```

- **Anchor Link**: Internal navigation using IDs.
  
  ```html
  <a href="#section1">Go to Section 1</a>
  <div id="section1">Content here</div>
  ```

---

### Images

- **Basic Image**: `<img>`
  
  ```html
  <img src="image.jpg" alt="Image description">
  ```

- **Responsive Image**: `width`, `height`
  
  ```html
  <img src="image.jpg" alt="Image description" width="100%" height="auto">
  ```

---

### Lists

- **Unordered List**: `<ul>` and `<li>`
  
  ```html
  <ul>
    <li>Item 1</li>
    <li>Item 2</li>
  </ul>
  ```

- **Ordered List**: `<ol>` and `<li>`
  
  ```html
  <ol>
    <li>First</li>
    <li>Second</li>
  </ol>
  ```

---

### Tables

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
      <td>Row 1 Col 1</td>
      <td>Row 1 Col 2</td>
    </tr>
  </tbody>
</table>
```

- `<table>`: Defines the table.
- `<thead>`, `<tbody>`, `<tfoot>`: Organizes table structure.
- `<th>`, `<td>`, `<tr>`: Defines table headers, data cells, and rows.

---

### Forms

```html
<form action="/submit" method="post">
  <label for="name">Name:</label>
  <input type="text" id="name" name="name" required>
  <input type="submit" value="Submit">
</form>
```

- **Form Fields**: `<input>`, `<select>`, `<textarea>`, `<button>`
- **Attributes**: `type`, `name`, `value`, `placeholder`, `required`

---

### Semantic HTML5 Elements

- **Layout Elements**: `<header>`, `<nav>`, `<section>`, `<article>`, `<footer>`
  
  ```html
  <header>Site Header</header>
  <nav>Navigation Menu</nav>
  <section>Main Content</section>
  <footer>Site Footer</footer>
  ```

- **Grouping Elements**: `<main>`, `<aside>`, `<figure>`, `<figcaption>`

---

### Media

- **Embed Images**: `<img>`
  
  ```html
  <img src="image.jpg" alt="Description">
  ```

- **Embed Video**: `<video>`
  
  ```html
  <video controls>
    <source src="video.mp4" type="video/mp4">
    Your browser does not support video.
  </video>
  ```

- **Embed Audio**: `<audio>`
  
  ```html
  <audio controls>
    <source src="audio.mp3" type="audio/mpeg">
    Your browser does not support audio.
  </audio>
  ```

---

### Best Practices

1. **Use Semantic HTML**: Use tags like `<article>`, `<section>`, `<nav>`, `<footer>` to improve accessibility and SEO.
  
2. **Alt Text for Images**: Always use descriptive `alt` attributes for images to support accessibility and SEO.

3. **Minimize Inline Styles**: Prefer external CSS for styling instead of using inline styles.

4. **Use Relative Paths**: Use relative paths for internal links and assets (e.g., `./images/pic.jpg`).

5. **Test Responsiveness**: Ensure your website is mobile-friendly by using responsive layouts (media queries) and testing across different devices.

6. **Validate HTML**: Use the [W3C HTML Validator](https://validator.w3.org/) to check for errors in your code.

---

This HTML cheatsheet provides a quick reference for essential HTML elements and best practices to follow when writing clean, efficient web pages.