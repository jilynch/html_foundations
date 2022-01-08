# HTML Foundations

Learn the foundations of HTML, a fundamental building block of everything on the web.

1. Introduction to HTML and CSS
2. Elements and Tags
3. HTML Boilerplate
4. Working with Text
5. Lists
6. Links and Images
7. Project: Recipes

## Elements and Tags

A typical element includes an opening tag with some attributes, enclosed text content, and a closing tag.
![HTML element structure](https://developer.mozilla.org/en-US/docs/Glossary/Element/anatomy-of-an-html-element.png)

## HTML Boilerplate

```html
<!DOCTYPE html>
<html>
	<head>
		<title>My First Webpage</title>
		<meta charset="UTF-8" />
	</head>

	<body>
		<h1>Hello World!</h1>
	</body>
</html>
```

## Working with Text

### Paragraphs

The `<p>` HTML element represents a paragraph. Paragraphs are block-level elements.

```html
<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
```

### Headings

The `<h1>` to `<h6>` HTML elements represent six levels of section headings. `<h1>` is the highest section level and `<h6>` is the lowest.

```html
<h1>Heading level 1</h1>
<h2>Heading level 2</h2>
<h3>Heading level 3</h3>
<h4>Heading level 4</h4>
<h5>Heading level 5</h5>
<h6>Heading level 6</h6>
```

### Strong Element

The `<strong>` HTML element indicates that its contents have strong importance, seriousness, or urgency. Typically this element is rendered by default using a bold font weight.

Use the `<b>` element to draw attention to certain text without indicating a higher level of importance.

```html
<p>
	... the most important rule, the rule you can never forget, no matter how much he cries, no matter how much he begs:
	<strong>never feed him after midnight</strong>.
</p>
```

### Em Element

The `<em>` HTML element marks text that has stress emphasis. The `<em>` element can be nested, with each level of nesting indicating a greater degree of emphasis. Typically this element is displayed in italic type.

Use the `<i>` element to mark text that is in an alternate tone or mood, which covers many common situations for italics such as scientific names or words in other languages.

```html
<p>Get out of bed <em>now</em>!</p>

<p>We <em>had</em> to do something about it.</p>

<p>This is <em>not</em> a drill!</p>
```

## Lists

### Unordered Lists

The `<ul>` HTML element represents an unordered list of items, typically rendered as a bulleted list.

#### Attributes

type:

-   `cricle`
-   `disc`
-   `square`

```html
<ul>
	<li>first item</li>
	<li>second item</li>
	<li>third item</li>
</ul>
```

### Ordered Lists

The `<ol>` HTML element represents an ordered list of items — typically rendered as a numbered list.

#### Attributes

-   `reversed`: specifies that the list’s items are in reverse order.
-   `start`: An integer to start counting from for the list items.
-   `type`: Sets the numbering type:
    -   a for lowercase letters
    -   A for uppercase letters
    -   i for lowercase Roman numerals
    -   I for uppercase Roman numerals
    -   1 for numbers (default)

```html
<ol type="i">
	<li>Introduction</li>
	<li>List of Greivances</li>
	<li>Conclusion</li>
</ol>
```

## Links and Images

### The Anchor element

The `<a>` HTML element (or anchor element), with its `href` attribute, creates a hyperlink to web pages, files, email addresses, locations in the same page, or anything else a URL can address.

```html
<a href="https://example.com">Website</a>
```

#### Attributes

-   `href`: The URL that the hyperlink points to.
    -   Sections of a page with fragment URLs
    -   Pieces of media files with media fragments
    -   Telephone numbers with tel: URLs
    -   Email addresses with mailto: URLs
-   `target`: Where to display the linked URL, as the name for a browsing context (a tab, window, or `<iframe>`).

    -   `_self`: the current browsing context. (Default)
    -   `_blank`: usually a new tab, but users can configure browsers to open a new window instead.
    -   `_parent`: the parent browsing context of the current one. If no parent, behaves as `_self`.
    -   `_top`: the topmost browsing context (the "highest" context that’s an ancestor of the current one). If no ancestors, behaves as `_self`.

### Absolute and Relative Links

-   Absolute Links: Links to pages on other websites on the internet

-   Relative Links: Links to other pages within our own website

### Images

The `<img>` HTML element embeds an image into the document.

```html
<img class="fit-picture" src="/media/cc0-images/grapefruit-slice-332-332.jpg" alt="Grapefruit slice atop a pile of other slices" />
```

-   The `src` attribute is required, and contains the path to the image you want to embed.
-   The `alt` attribute holds a text description of the image, which isn't mandatory but is incredibly useful for accessibility — screen readers read this description out to their users so they know what the image means. Alt text is also displayed on the page if the image can't be loaded for some reason: for example, network errors, content blocking, or linkrot.
