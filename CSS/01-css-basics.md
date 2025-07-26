# CSS Basics
## What You Will Learn
- [What is CSS](#what-is-css)
- [Including CSS in a Web Page](#including-css-in-a-web-page)
- [Creating and Linking External Stylesheets](#creating-and-linking-external-sytlesheets)
- [CSS Rules](#css-rules)
- 

## What is CSS
CSS (Cascading Style Sheets) is language used to style and format the presentation of HTML elements in web documents.

## Including CSS in a web page
### How to bring CSS to Web Pages
There are three ways to introduce CSS to web pages:
#### Inline Styles
Using inline styles means adding styles directly to individual HTML elements. 
Inline styles are applied directly to individual elements, like colouring a specific word in a sentence.

```HTML
<p style="color: blue;">
  Hell0, CSS!
</p>
```
 #### Internal Styles
 Internal Styles refers to a tag called `<style>` placed within the `<head>` section.
 It lets you embed CSS rule directly within the HTML document. 
 This can be particularly useful when you're dealing with a single-page project.

 ```HTML
<head>
  <style>
    p {
      color: red;
    }
  </style>
</head>

<body>
  <p>Hello, CSS!</p>
</body>
```

#### External Sheets
Using external sheets means creating CSS files(.css) that you link to your HTML.

This method keeps you styles organised and consistent across multiple pages. It'ss a popular choice for large projects.  

index.html:
```HTML
<head>
  <link rel="stylesheet" type="text/css" href="styles.css">
</head>

<body>
  <p>Hello, CSS!</p>
</body>
```
styles.css:
```CSS
p {
  color: green;
}
```

## Creating and Linking External Sytlesheets
Creating and deploying a CSS file involves a few important steps to ensure a clean and organised coding process.

### Setp 1: Plan and Design
Start by planning the visual of your website. Consider the color shceme, typography, layout and overall aesthetics. Create a design prototype or mockup to have a clear vision of how you want your website to look like.

### Step 2: Choose a Text Editor or IDE
Select a reliable text editor or intergrated development environment (IDE) for writing of HTML and CSS code. 

### Step 3: Create a Directory Structure
Set-up a well-organised directory structure for your project. Create separate folders for HTML files, CSS files, images and other assets. This structure will make it easier to manage and maintain your project as it grows.

### Step 4: Create a CSS File
Within your CSS folder, create a new CSS file. Give it a meaningful name related to its purpose, like "styles.css" or "main.css".

### Step 5: Wirte CSS Code
Open CSS file and start writing the styling rules based on your design. 
Divide your CSS rules into sections for different parts of the website (heaader, footer, nagivation, etc.) to maintain organisation.

For example:
```HTML
/* Styles for the header section */
.header {
  background-color: #333;
  color: white;
  padding: 20px;
}

/* Styles for the navigation menu */
.nav {
  display: flex;
  justify-content: space-between;
  padding: 10px;
}

.nav li {
  list-style: none;
  margin-right: 15px;
}

/* Styles for the main content */
.main-content {
  font-size: 16px;
  line-height: 1.5;
  padding: 20px;
}

/* Styles for the footer section */
.footer {
  background-color: #f4f4f4;
  padding: 15px;
  text-align: center;
}
```

### Step 6: Implement Responsive Design
Make your CSS file responsive by using *media queries*. This ensures that your website looks and functions well on various screen  sizes and devices.

> *media queries*: CSS features that let you adjust how your webpage looks on different devices by applying specific styles based on factors like screen size.

### Step 7: Minify and Optimize
Before deploying CSS file, consider minifying and optimizing it.
**Minification** removes any unnecessary spaces and comments to reduce file size, which improves loading speed.

### Step 8: Deploy to a Web Server
To deploy your CSS file, you need a web server. After choosing the appropirate hosting option, upload your css file to the appropriate directory on the server.

### Step 9: Link CSS in HTML
In your HTML files, link your CSS file using the `<link>` element. Place this element in the`<head>` section of each HTML file.
```HTML
<!-- index.html -->
<!DOCTYPE html>
<html>
<head>
  <link rel="stylesheet" type="text/css" href="styles.css">
</head>
<body>
  <h1>Welcome to My Website</h1>
  <p>This is a paragraph of text.</p>
</body>
</html>
```
### Step 10: Test and Debug
After deploying your CSS file, thoroughly test your website on different browsers and devices to ensure that the styling looks consistent and functions correctly.


## CSS Rules
CSS employs a very straightforward syntax that consists of CSS Rules.

Basic Structure of a CSS rule:
```
selector {
  property: value;
  another-property: another-value;
}
```
### Selectors, Properties and Values
| Syntax Component | Definition |
|--- | --- |
|Selector| Specifies which HTML elements the rule will apply to. For Example:  element selector `p` will target all `<p>` elements|
| Property| Defines the aspect you want to to style, such as color, font-size, margin, etc|
| Value | Determines the styling details.Example:  `color: blue;`|
| Declaration Block | A set of property-value pairs enclosed in curly braces `{}`. |

### Combining Selectors
When working with CSS, you'll frequently come accross situations where you need to apply the same styles to multiple elements that share common attributes.

Syntax:
```
selector1, selector2, selector3 {
  property: value;
}
```
> Note:
> Many properties in CSS can take multiple values separated by commans within the property-value pair.  
> Example:
> ```
> p {
>  font-family: "Roboto", Arial, sans-serif;
> }
> ```
