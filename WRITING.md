# Writing Guide

Content on the KOTOR Community Portal is written in **Markdown**, a lightweight and popular markup language. During publishing, the KOTOR Community Portal toolchain converts these Markdown documents into the HTML documents that are visible on the website. This makes it possible to edit the content of a webpage in Markdown separately from its presentation in HTML. In this way, one does not need to know anything about HTML to be able to contribute content to our website.

Our Markdown parser follows the [CommonMark](https://commonmark.org/) specification of Markdown and has a few custom extensions. GitHub Flavored Markdown also follows the CommonMark specification, so it is possible to edit content directly in your browers using GitHub's web editor.

This document will go over the Markdown syntax for our most common use cases. This is by no means a comprehensive description of Markdown. [GitHub's writing guide](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax) is a good resource for additional Markdown syntax not covered by this document. Our Markdown parser does not support all of GitHub Flavored Markdown's extensions, but there is a lot of overlap, so their guide is still a good resource.

## Headings

A heading is the title of a section or subsection on a webpage. There are six heading levels. To create a heading, write between one and six hashtags `#` followed by a space and the heading text. The number of hashtags determines the heading level.

```
# Onderon

## Description

## History

### Early History

### The Beast Wars and the Naddist Uprising

### The Mandalorian Wars and the Jedi Civil War

### The Onderon Civil War
```

_You must include a space between the final hashtag and the heading text._ Some flavors of Markdown, such as Reddit's, do not require this. GitHub Flavored Markdown and our Markdown parser follow the CommonMark specification, which does.

### Usage

- Use only one first-level heading per page. This heading should describe the content of the entire page.
- Do not use headings merely to emphasize text. Prefer other styling options such as bold and italics where applicable.
- Avoid styling heading text, like making all heading text bold. Headings are styled differently than other text through CSS, so it is not necessary to make them stand out by applying additional styling in Markdown, and doing so will lead to inconsistencies. Still follow conventional formatting rules where applicable. For example, italicize ship names such as the _Ebon Hawk_.

## Styling Text

The following styling options are supported:

| Style       | Syntax                 | Example                                   | Output                                               |
| :---------- | :--------------------- | :---------------------------------------- | :--------------------------------------------------- |
| Bold        | `** **` or `__ __`     | `**This text is bold.**    `              | **This text is bold.**                               |
| Italic      | `* *` or `_ _`         | `_This text is italicized_.`              | _This text is italicized_                            |
| Bold Italic | `*** ***` or `___ ___` | `***This text is bold and italicized.***` | ***This text is bold and italicized.***              |
| Deleted     | `~~ ~~`                | `~~This text was deleted.~~`              | <img src="https://github.com/KOTOR-Community-Portal/web-content/assets/46898647/a28c5871-f376-485f-8e16-cf358fd1a3e6" alt="This text was deleted." height="30px" /> |
| Inserted    | `++ ++`                | `++This text was inserted.++`             | <img src="https://github.com/KOTOR-Community-Portal/web-content/assets/46898647/38bfb9f2-6b79-4350-9cc5-e87631339a9a" alt="This text was inserted." height="30px" /> |
| Marked      | `== ==`                | `==This text was marked.==`               | <img src="https://github.com/KOTOR-Community-Portal/web-content/assets/46898647/0f1d80ef-2138-4fd3-ae79-7acda7b729dc" alt="This text was marked." height="30px" /> |
| Subscript   | `~ ~`                  | `C~3~H~5~N~3~O~9~`                        | C<sub>3</sub>H<sub>5</sub>N<sub>3</sub>O<sub>9</sub> |
| Superscript | `^ ^`                  | `a^2^ + b^2^ = c^2^`                      | a<sup>2</sup> + b<sup>2</sup> = c<sup>2</sup>        |
| Spoiler     | `>! !<`                | `>!This text is a spoiler.!<`             | <img src="https://github.com/KOTOR-Community-Portal/web-content/assets/46898647/5d465a7f-47e0-463c-8591-7c069a136d3d" alt="This text is a spoiler." height="30px" /> |

_The **marked**, **subscript**, **superscript**, and **spoiler** extensions are not supported by GitHub Flavored Markdown and will not preview correctly on GitHub's web editor._

## Links

You can create a link by wrapping the text you want display in square brackets `[ ]` and wrapping the URL in parentheses `( )`.

`[KOTOR Community Portal lore questions](https://kotor.neocities.org/faq/lore.html)`

[KOTOR Community Portal lore questions](https://kotor.neocities.org/faq/lore.html)

### Relative Paths

If you are linking to a webpage on the KOTOR Community Portal, you do not need to include the entire URL. The KOTOR Community Portal server is able to find the same webpage using a relative path. A relative URL starts with a forward slash `/` and includes only the part of the URL that normally appears after the `kotor.neocities.org` domain.

The following links point to the same webpage:

`https://kotor.neocities.org/faq/lore.html`

`/faq/lore.html`

### index.html

If a KOTOR Community Portal link points to a directory instead of a file, the server will attempt to load the directory's default webpage, `index.html`. You do not need to include the `index.html` part of the URL when linking to this page.

The following links point to the same webpage:

`/modding/mod_builds/index.html`

`/modding/mod_builds/`

### URL Fragments

You can link to a specific part of a webpage using a URL fragment. A URL fragment is an optional part at the end of a URL.

A URL fragment beings with a hash tag `#` and is followed by the identifier of an element on the webpage.

`/faq/k2.html#Bug_Support`

The KOTOR Community Portal's toolchain automatically generates identifiers for important elements on each page so they may be linked to. _Be careful when changing a heading, as this will change its identifier and break any existing links to it._

## Images

You can insert an image by writing an exclamation mark `!` followed by the image's alt text wrapped in square brackets `[ ]` and the image's URL wrapped in parentheses `( )`. Alt text is a short description of the image which is used whenever the image itself is not displayed, such as when the page is read from a screen reader.

`![Example image stolen from GitHub's writing guide](https://docs.github.com/assets/cb-39745/mw-1440/images/help/writing/image-rendered.webp)`

<img src="https://docs.github.com/assets/cb-39745/mw-1440/images/help/writing/image-rendered.webp" alt="Example image stolen from GitHub's Markdown guide" height="100px"/>

## Line Spacing Sequences

Our Markdown parser trims blank lines, so any extra line spacing between paragraphs or sections of text will be ignored and will not be included in the output HTML document. If you want to insert extra line spacing, there are a few alternative options:

| Sequence       |Syntax                  | HTML Output | Description                                                                  |
| :------------- |:---------------------- | :---------- | :--------------------------------------------------------------------------- |
| Thematic Break |`___` or `---` or `***` | `<hr />`    | A horizontal rule                                                            |
| Line Break     |`__` or `--` or `**`    | `<br />`    | A line with no content and the same height as a normal line                  |
| Empty Line     |`__\` or `--\` or `**\` | `<p></p>`   | A line with no content and zero height, but with the margin of a normal line |

Up to three spaces may be appear before the sequence. There may be spaces and tabs between characters in the sequence and after the sequence. No other characters may appear on the same line.

```
Rise
___

Decline and Fall

```

Rise

___

Decline and Fall

_The **line break** and **empty line** extensions are not supported by GitHub Flavored Markdown and will not preview correctly on GitHub's web editor._

## Tables

You can organize information in tables using pipe `|` and hyphen `-` characters. Pipes separate the table's columns, while hyphens separate the header row from the other rows.

The default text alignment is centered for header cells and left for all other cells. You can add a colon `:` to the left or right of a column header separator to make the entire column left- or right-aligned. Including both will make the column center-aligned.

```
| Attribute    | Score | Modifier |
| :----------- | :---: | :------: |
| Strength     | 16    | +3       |
| Dexterity    | 10    | -        |
| Constitution | 12    | +1       |
| Intelligence | 8     | -1       |
| Wisdom       | 15    | +2       |
| Charisma     | 14    | +2       |
```

| Attribute    | Score | Modifier |
| :----------- | :---: | :------: |
| Strength     | 16    | +3       |
| Dexterity    | 10    | -        |
| Constitution | 12    | +1       |
| Intelligence | 8     | -1       |
| Wisdom       | 15    | +2       |
| Charisma     | 14    | +2       |
