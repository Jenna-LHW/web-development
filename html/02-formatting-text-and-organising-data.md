# Formatting Text and Organising Data

## What You will Learn

- [Headings](#headings)
- [Paragraphs and Text Formatting - Part 1](#paragraphs-and-text-formatting-part-1)
- [Paragraphs and Text Formatting - Part 2](#paragraphs-and-text-formatting-part-2)
- [Paragraphs and Text Formatting - Part 3](#paragraphs-and-text-formatting-part-3)
- [Paragraphs and Text Formatting - Part 4](#paragraphs-and-text-formatting-part-4)
- [Lists](#lists).
- [Tables](#tables).

## Headings
HTML headings are special elements in an HTML document that are used to define the heading or title of a section or page.
They provide structure and hierachy to a web page.

As mentioned before, there are six levels of HTML headings, ranging from `<h1>` to `<h6>`.

### Heading Sizes
The size of headings is defined by HTML tags `<h1>` to `<h6>`, but the actual display size can vary depending on the browser and the device used to view the page.

Typical font size for the different heading levels:
- `<h1>`: 32px 
- `<h2>`: 24px
- `<h3>`: 18px
- `<h4>`: 16px
- `<h5>`: 14px
- `<h6>`: 12px

## Paragraphs and Text Formatting - Part 1
### The `<p>` Tag and Inline Formatting
In HTML, paragraphs are defined using the `<p>` tag.
The `<p>` tag is a **block-level** element, which means that it takes up the **entire width** of the container in which it is placed.

To create a paragraph, you can use the opening `<p>` tag before the text and the closing `</p>` tag after the text that you want to display as a paragraph.

### Formatting Text with Inline Tags
Here are some of the most common tags that can be used for formatting text within a paragraph:

#### The `<strong>` Tag
The `<strong>` tag is used to make the enclosed text **bold**.   For example:
```HTML
<p> This is  some <strong>important</strong> text.</p>
```

#### The `<em>` Tag
The `<em>` tag is used to make the enclosed text *italic*.
```HTML
<p>This is some text that requires <em>emphasis</em>.</p>
```

#### The `<u>` Tag
The `<u>` tag is used to underline the enclosed text.
```HTML
<p>This is some text that needs to be <u>underlined</u>.</p>
```

#### The `<sup>` Tag
The `<sup>` tag is used to make the enclosed text superscript.
```HTML
<p>1<sup>st</sup>, 2<sup>nd</sup>, and 3<sup>rd</sup></p>
```
Output:
> <p>1<sup>st</sup>, 2<sup>nd</sup>, and 3<sup>rd</sup></p>

#### The `<sub>` Tag
The `<sub>` tag is used to make the enclosed text subscript.
```HTML
<p>The chemical formula for water is H<sub>2</sub>O.</p>
```
Output:
> <p>The chemical formula for water is H<sub>2</sub>O.</p>

#### The `<del>` Tag
The `<del>` tag is used to strike through text.
```HTML
<p>Special Price: <del>$100</del> $75.</p>
```

The `<mark>` Tag
The `<mark>` tag is used to highlight text with a background color, indicating that it is of special importance.
```HTML
<p>The deadline for submitting the report is <mark>Monday, March 12th</mark>.</p>
```
Output:
> <p>The deadline for submitting the report is <mark>Monday, March 12th</mark>.</p>
