
# TITLE

## CSS File Linking with HTML File

### Introduction

Hypertext Markup Language (HTML) forms a fundamental aspect of web development, making it an essential component of the software engineering journey for beginners. Despite its significance, it cannot function in isolation; it requires other web technologies to be well organized and linked to the HTML file. In this article, I will explain the necessary process for linking an HTML file with CSS. As you read through this content, consider taking a moment to enjoy a cup of water.

### Table of Contents

1. What is HTML and Its Uses
2. Where Can We Write HTML Files?
3. What Are IDEs?
4. Understanding the HTML Boilerplate
5. How to Link HTML with CSS File and Types of Linking

### Prerequisites

To maximize the value of this article, it's important to grasp the fundamental HTML boilerplate and approach the material with a keen desire to learn.

### What is HTML and Its Uses?

HTML, short for Hypertext Markup Language, serves as the foundational language in web development, defining the structure of web pages.

The term "Hypertext" was coined by Ted Nelson in 1965 and refers to text containing links to other text. (source: [W3C](https://www.w3.org/WhatIs.html))

"Markup" pertains to a character set encoding system, consisting of identical symbols that create structure on web pages.

HTML, functioning as a markup language, serves to define the structural representation of web pages.

### Where Can We Write HTML Files?

Just as each form of writing requires a specific environment, the same holds true for HTML. It necessitates a development environment referred to as an Integrated Development Environment (IDE). This leads us to our next topic: "What is an IDE?"

### What is an IDE?

An Integrated Development Environment (IDE) serves as a platform for software engineers to develop and debug code. There are two main types of IDEs:

- Online IDEs
- Offline IDEs

#### Online IDEs

These web-based development environments can be utilized without local installation. They are often used for smaller projects due to their simple accessibility. Examples include CodePen, Sandcodebox, and Replit.

#### Offline IDEs

As the name suggests, these IDEs are used offline and don't require an internet connection. However, they require setup before use, unlike their online counterparts. Examples of offline IDEs include Visual Studio Code, Bracket, Atom, and Sublime. Visual Studio Code is particularly recommended for various reasons beyond the scope of this article.

### Understanding the HTML Boilerplate

The visual representation of the HTML boilerplate:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>HTML 5 Boilerplate</title>
    <link rel="stylesheet" href="style.css">
  </head>
  <body>
    <script src="index.js"></script>
  </body>
</html>
```


- `<!DOCTYPE html>`: The DOCTYPE at the beginning of the code signifies an HTML 5 declaration, allowing browsers to recognize the syntax used in the subsequent HTML file as HTML 5. While not mandatory, it demonstrates the programmer's expertise in development.

- `<html> </html>`: This encloses the root element of the HTML file, encompassing all other elements in the document.

- *The Head Element*: Comprising meta tags, title elements, and link elements, the head element is primarily used by browsers to glean information about the web page.

- *Link Element*: This element facilitates the linkage of our HTML file with other files for implementing special features. Further discussion on this element follows in the subsequent section, as it is the focus of this article.

- *The Body Element*: The most impactful aspect of the HTML file, the body element comprises content displayed on the website. It's crucial for providing the best user experience.

### How to Link HTML with CSS File and Types of Linking

Linking an HTML file with CSS and JavaScript files involves various types. The primary three widely recognized types are as follows:

1. Inline styling
2. Internal styling
3. External Styling

- *Inline Styling*: CSS syntax is directly written into HTML code as an attribute. The code snippet below illustrates its usage.

```html
<h1 style="color:blue;">A Blue Heading</h1>
```


Inline styling isn't always recommended, as larger projects can result in messy code that's challenging to debug.

- *Internal Styling*: This type of styling is written in the head section of the code, between the opening and closing style tags.

```html
<style>
  body {background-color: powderblue;}
  h1   {color: blue;}
  p    {color: red;}
</style>
```


Internal styling is suitable primarily for smaller projects.

- *External Styling*: External Styling is the industry standard for writing CSS in a project. It involves writing CSS in a separate file, enhancing code readability and organization. Developers gain flexibility for debugging when needed. To utilize external styling and connect HTML to CSS, the Link tag is employed. This Link Element features attributes like href (containing the file reference) and rel (indicating the file's relationship to the HTML).

```html
<link rel="stylesheet" href="/html/styles.css">
```


This method is most widely used, enhancing code professionalism, readability, and collaboration among future developers.

### Conclusion

This article has explored how to link a stylesheet to an HTML file, highlighting the best practice among the various types of linking discussed. Through clear explanations, achieving effective CSS styling linking becomes more attainable.