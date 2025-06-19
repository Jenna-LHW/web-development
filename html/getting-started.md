# Getting Started with HTML

## What you will learn

- [Introduction to HTML](#introduction-to-html)
- [First HTML File](#first-html-file)
- [HTML Syntax](#html-syntax)
- [HTML Syntax: Attributes and Values](#html-syntax-attributes-and-values)
- [HTML Syntax: HTML, Head and Body Tags](#html-syntax-html,-head-and-body-tags)
  
## Introduction to HTML
**What is HTML?**  
HTML = HyperText Markup Language
- **Hypertext** refers to text that contains links to other documents or resources.
- **Markup** refers to the annotations or tags that are used to define the structure and formattning of content in a document.
- **Language** refers to the system of rules and syntax used to write and interpret the **markup** in a consisent and standardized manner.

**Setting Up An HTML Development Environment**  
To start writting and testing HTML code, tools such as a **text editor** and a **web browser** will be needed.
> What I am using:
> - Text Editor: VS code
> - Web Browser: Microsoft Edge

## First HTML File
**Step 1 - Create an HTML file**  
Open text editor and create new file. Save the file using a name and the `.html` extension. For example, `sample.html`.

**Step 2 - Write the HTML code**
Inside the HTML file, you can start adding you code.

```HTML
<!DOCTYPE html>
<html>
<head>
  <title>My First Web Page</title>
</head>
<body>
  <h1>Hello, World!</h1>
  <p>This is my first web page.</p>
</body>
</html>
```

**Step 3 - Save an open the HTML file**
Save the HTML file and navigate to the location where it is saved.  Click on the file and it will open on your default web browser.

## HTML Syntax
### The DOCTYPE declaration
The DOCTYPE declaration is an integral part of HTML syntax and an important element in an HTML document that helps web browsers understand how to interpret the document's content.  
The DOCTYPE declaration is a special line of code that should appear **at the beginning of an HTML document**, before any other content or elements.  
```HTML
<!DOCTYPE html>
```
This tells the web browser that the document is written in **HTML5**, and the browser will therefore expect to see HTML5 syntax and features throughout the rest of the document.  

### Elements and Tags
HTML is made up of a series of **elements**, which are defined by **tags**.   

**HTML Element**
An HTML element is a part of a webpage, like a paragraph or an image.  
Elements tell the web browser how to display the content.

**HTML Tags**
Tags are the markers that define the start and the end of an element. 

For example, a paragraph is created with a `<p>` tag, indicating the start, and a `</p>` tag, marking the end.

```HTML
  <p>              content             </p>
opening tag  content in between  closing tag
```

**Understanding Tags and Elements**  
The basic structure of an HTML element includes:
- the opening tag (`<tag>`)
- the content itself
- the closing tag (`</tag>`)

The **opening tag** marks the start of an element and can include [attributes](#html-syntax-attributes-and-values)

**Self-Closing Tags** are elements, like the image element, that *don't contiain content* and therefore *don't have a closing tag*.
For example,
```HTML
<img src="image.jpg" alt="Description of the image">
```

### Block-Level and Inline Elements
In HTML5, there are two types of elements:
- block-level elements
- inline elements

**Block-Level Elements** are used to create the main structutre of a web page, such as headers, paragraphs and lists.
They start on a new line and take up the full width of the page. 
This means that any content places inside a block-level element will create a new block of content, separate from the content before or after it.

Example of block-Level elements include:
- `<h1>` through `<h6>` for headings
- `<p>` for paragraghs
- `<ul>` and `<ol>` for lists
- `<div>` for grouping content

**Inline Elements** are used to style content within block-level elements, such as links and images.
They don't don't start on a new line and only take up as much as needed to display their content. 
This means that multiple inline elements can appear on the same line, separated by a space.

Examples of inline elements include:
- `<a>` for links
- `<img>` for images
- `<span>` for styling content

### HTML Comments
HTML comments are a way to add notes or remarks in an HTML document that won't be visible to the user. Comments can be used to explain what certain parts of the code do or to temporarily disable parts of the code during development.
To create a comment, you simply need to enclose the text you want to comment out between `<!--` and `-->`.

For example,
```HTML
<!--This is a comment -->
```
> **Tips**  
> If you are using vs code, your can press `ctrl` + `/` to comment  and uncomment any line!

## HTML Syntax: Attributes and Values
**Attributes** are extra details that configure or adjust the element's behaviour.  
They have a name and a value, separated by an equal sign, with the value enclosed in quotes.   

For example,
```HTML
<a class="hero" id="1"> content </a>
```

### Global vs Element-Specific attributes
HTML attributes can be broadly classified into two categories:
- **global attributes** can be applied to any HTML element. They are useful for a wide range of purposes, such as assigning unique identifiers, adding clases for styling or providing additional information about an element.  
 Example: `id`, `class`, `style` and `title`.

- **element-specific attributes** are specific to particular HTML elements and cannot be used with all elements.They provide functionality of modify the behaviour of specific elements.  
  Example:
  - `href`: specific to `<a>` elements
  - `scr`:  specific to `<img>` and media elements
  - `type`: specific to `<input>` elements
 
## HTML Syntax: HTML, Head and Body Tags
**HTML tag** (`<html>`) is one of the moset important tags in an HTML document, as it defines the entire web page and serves as the starting point for every HTML document.
It informs the browser that the document is an HTML document and is the first tag in every HTML document.  

The HTML tag has an opening and a closing tag. Everything in the document appears between these two tags and it does not have any attributed associated with it.

```HTML
<!DOCTYPE html>
<html>
   <!-- The hidden content of an HTML document: the head section will go here. -->
   <!-- The visible content of an HTML document: the body section will go here. -->
</html>
```
The **Head section** is an important component of an HTML document that contains information used by the browser to display and interact with the web page.
It can optimise the web page for search engined and additional context to users. The *head section* is hidden from the user's view and does not appear on the web page. (*It is a background portion of the document that operates behind the scenes*)

Some of the key pieces of information that can be included in the *head section* are:
- **Page title**, the title of the web page that appears in the title bar of the broweser and is used by search engined to display the page title in search results.
  Example: `<title>My Web Page</title>`
- **Meta Data**, includes the description and keywords that are used by search engines to index and rank the web page, instructions for web crawlers how to index and dislay the web page or information about the author and creation date of the page.
  Example: `<meta name="author" content="Peter Jackson">`  
- **Links to external files**, which includes CSS stylesheets and JavaScript file that add styling and functionality to the web page.  
  Example: `<link rel="stylesheet" href="styles.css"><script src="script.js"></script>`
- **Character encoding**, which tells the browser what character set to use when displaying the web page.
  Example: `<meta charset="UTF-8">

Here is an example of the head section in an HTML document:
```HTML
<!DOCTYPE html>
<html>
   <head>
      <title>My Web Page</title>
      <meta name="description" content="This is a website about soccer!">
      <link rel="stylesheet" href="styles.css">
      <script src="script.js"></script>
   </head>
   <!-- The visible content of an HTML document: the body section will go here. -->
</html>
```
The **body section** is the part of an HTML document that contains the visible content of the web page.  
It contains the actual content that the user will see and interact with.

Examples of content that can be included in the body section:
- Text
- Images
- Videos
- Forms
- Links
- Lists
- Tables

Here is an example of the body section in an HTML document:
```HTML
<!DOCTYPE html>
<html>
   <head>
      <title>John Smith Photography</title>
      <meta name="description" content="John Smith Photography specializes in capturing authentic and compelling images that tell the story of your business, project, or cause.">
      <link rel="stylesheet" href="styles.css">
      <script src="script.js"></script>
   </head>
   <body>
      <h1>Bringing Your Brand to Life with Striking Visuals</h1>
      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
      <img src="/resources/media/html-ess-1-7-1-apple-photo.jpg" alt="Apple photo">
   </body>
</html>
```

> **Tips**  
> If you are using vs code, just type `!` followed by `tab` or `Enter`  it will give you this:
> ```HTML
> <!DOCTYPE html>
> <html lang="en">
> <head>
>    <meta charset="UTF-8">
>    <meta name="viewport" content="width=device-width, initial-scale=1.0">
>    <title>Document</title>
> </head>
> <body>
>    
> </body>
> </html>
> ```
