# Formatting Text and Organising Data

## What You will Learn

- [Headings](#headings)
- [Paragraphs and Text Formatting - Part 1](#paragraphs-and-text-formatting---part-1)
- [Paragraphs and Text Formatting - Part 2](#paragraphs-and-text-formatting---part-2)
- [Paragraphs and Text Formatting - Part 3](#paragraphs-and-text-formatting---part-3)
- [Paragraphs and Text Formatting - Part 4](#paragraphs-and-text-formatting---part-4)
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

#### The `<mark>` Tag
The `<mark>` tag is used to highlight text with a background color, indicating that it is of special importance.
```HTML
<p>The deadline for submitting the report is <mark>Monday, March 12th</mark>.</p>
```
Output:
> <p>The deadline for submitting the report is <mark>Monday, March 12th</mark>.</p>

## Paragraphs and Text Formatting - Part 2
When you want to adda quote to your HMTML document, you can use two tags:
- the `<q>` tag
- the `<blockquote>` tag

### The`<q>` Tag
The `<q>` tag is used for short, inline quotes.
```HTML
<p><q>The only way to do great work is to love what you do.</q> - Steve Jobs</p>
```
Output:
> <p><q>The only way to do great work is to love what you do.</q> - Steve Jobs</p>

### The `<blockquote>` Tag
The `<blockquote>` tag is used for lonfer, block quotes.
```HTML
<p>As Albert Einstein once said:</p>
<blockquote>
  <p>"Imagination is more important than knowledge. Knowledge is limited. Imagination encircles the world. The true sign of intelligence is not knowledge but imagination."</p>
</blockquote>
<p>This quote speaks to the idea that creativity and original thinking are more important than simply accumulating knowledge. It suggests that being able to see beyond what is already known and to imagine new possibilities is a key characteristic of intelligence.</p>
```
Ouput:
> <p>As Albert Einstein once said:</p>
> <blockquote>
> <p>"Imagination is more important than knowledge. Knowledge is limited. Imagination  encircles the world. The true sign of intelligence is not knowledge but imagination."</p>
> </blockquote>
> <p>This quote speaks to the idea that creativity and original thinking are more important than simply accumulating knowledge. It suggests that being able to see beyond what is already known and to imagine new possibilities is a key characteristic of intelligence.</p>

### The `<cite>` Tag
When you want to mark up the title or source of a book, film, song, or any other creative work, provide attribution or credit for an idea or information, or indicate a reference to another source, you can use the `<cite>` element.

```HTML
<p>I recently read <cite>The Great Gatsby</cite> by F. Scott Fitzgerald.</p>
```

The content withing the `<cite>` element is typically displayed in *italic* style.

### The `<cite>` Attribute
When using quotes, it's important to attribute the source of the quotes, typically by providing a URL.

```HTML
<p>As Steve Jobs once said, <q cite="https://www.brainyquote.com/quotes/steve_jobs_416096">Innovation distinguishes between a leader and a follower.</q></p>
```

The `<cite>` attribute doesn't have a visible effect in a web browser, but it can be used by screen readers to provide additional context.

### The `<footer>` Tags
Another way to provide more context for a quotation is to use the `<footer>` tag, which is a semantic tag that helps search engines and screen readers understand the content of the page.

```HTML
<blockquote>
<p>The more that you read, the more things you will know. The more that you learn, the more places you'll go.</p>
<footer>- Dr. Seuss</footer>
</blockquote>
```
Output:
> <blockquote>
<p>The more that you read, the more things you will know. The more that you learn, the more places you'll go.</p>
<footer>- Dr. Seuss</footer>
</blockquote>

## Paragraphs and Text Formatting - Part 3
### Line Breaks
A line break is a simple element that creates a new line of text within a block-level element. This is typically represented by the `<br>` tag and is used to separate lines of text.

**Note:** The `<br>` tag is an empty element, meaning it doesn't require a closing tag.
```HTML
<p>This is the first line.<br>This is the second line.</p>
```
Output:
> <p>This is the first line.<br>This is the second line.</p>

### Horizontal Rules
A horizontal rule is a visual elemet tahat ceatesa horizontal line across the width of a block-level element. It is typically used to separate sections of content witing a page.

The `<hr>` element is self-closing and does not require a closing tag.
```html
<p>This is some text above the line.</p>
<hr>
<p>This is some text below the line.</p>
```
Output:
> <p>This is some text above the line.</p>
> <hr>
> <p>This is some text below the line.</p>

## Paragraphs and Text Formatting - Part 4
### The `<code>` Tag
The `<code>` tag is used to display inline code snippets.
When used, the text inside the `<code>` tag is displayed in a monospaced font.

```HTML
<code>Hello, World!</code>
```
Output:
> <code>Hello, World!</code>

### The `<pre>` Tag
The `<pre>` is used to display preformatted text like computer code, poetry or songs lyrics in HTML.

```HTML
<pre>Hello, World!
What a sight to see,
A vast and endless web,
Connecting you and me.</pre>
```
Output:
> <pre>Hello, World!
> What a sight to see,
> A vast and endless web,
> Connecting you and me.</pre>

### The `<kbd>` Tag
The `<kbd>` tag is used to display keyboard input. The text enclosed within the `<kbd>` tad is typically displayed in a monospace font, sometimes in a rectangular box, which indicates that it represents keyboard input. 
```HTML
<o>To copy you need to press: <kbd> Ctrl + C</kbd> </p>
```
Output:
> <o>To copy you need to press: <kbd> Ctrl + C</kbd> </p>

### The `<samp>` Tag
The `<samp>` tag is used to indicate output in a web page. When text is enclosed within the <samp> tag, it is typically displayed in a monospace font and emphasized in some way, such as bold or italicized, to indicate that it represents sample output.

```HTML
<samp>Invalid username or password.<samp>
```

Output:  
<samp>Invalid username or password.<samp>

## Lists
There are three types of lists in HTML:
- unordered lists,
- ordererd lists, and
- definition lists.

### Unordered Lists
Unordered lists are created with the `<ul>` tag, and are used to display a list of items with no particular order. Each item in the list is represented by the `<li>` tag.

```HTML
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>
```

Output:
><ul>
>    <li>Item 1</li>
>    <li>Item 2</li>
>    <li>Item 3</li>
></ul>

### Ordered Lists
Ordered lists are created with the `<ol>` tag, and are used to display a list of items in a specific order. Just like in the case of unordered lists, each item in an ordered list is represented by the `<li>` tag.

```HTML
<ol>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item</li>
</ol>
```
Ouput:
> <ol>
>  <li>First item</li>
>  <li>Second item</li>
>  <li>Third item</li>
> </ol>

### Definition Lists
Definition lists are created with the `<dl>` tag, and are used to display a list of terms and their definitions. Each term is represented by the <dt> tag, and each definition is represented by the `<dd>` tag.
```html
<dl>
  <dt>Term 1</dt>
  <dd>Definition 1</dd>
  <dt>Term 2</dt>
  <dd>Definition 2</dd>
  <dt>Term 3</dt>
  <dd>Definition 3</dd>
</dl>
```
Output:
><dl>
>  <dt>Term 1</dt>
>  <dd>Definition 1</dd>
>  <dt>Term 2</dt>
>  <dd>Definition 2</dd>
>  <dt>Term 3</dt>
>  <dd>Definition 3</dd>
></dl>

### Nested Lists
HTML allows you to nest lists within other lists. This means you can create a hierarchy of information, where sub-lists are indented to show they belong to a parent list item.

To create a nested list, simply place a new `<ul>` or `<ol>` element within an existing `<li>` element.
```HTML
<ul>
  <li>First item</li>
  <li>Second item
    <ul>
      <li>Sub-item 1</li>
      <li>Sub-item 2</li>
    </ul>
  </li>
  <li>Third item</li>
</ul>
```
Output:
><ul>
>  <li>First item</li>
>  <li>Second item
>    <ul>
>      <li>Sub-item 1</li>
>      <li>Sub-item 2</li>
>    </ul>
>  </li>
>  <li>Third item</li>
></ul>
