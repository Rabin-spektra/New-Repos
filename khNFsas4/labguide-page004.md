# Complete Markdown Syntax Guide

## Table of Contents
1. [Headings](#headings)
2. [Paragraphs and Line Breaks](#paragraphs-and-line-breaks)
3. [Text Formatting](#text-formatting)
4. [Lists](#lists)
5. [Links](#links)
6. [Images](#images)
7. [Code](#code)
8. [Blockquotes](#blockquotes)
9. [Horizontal Rules](#horizontal-rules)
10. [Tables](#tables)
11. [Task Lists](#task-lists)
12. [Strikethrough](#strikethrough)
13. [Subscript and Superscript](#subscript-and-superscript)
14. [Highlighting](#highlighting)
15. [Emojis](#emojis)
16. [HTML Elements](#html-elements)
17. [Escape Characters](#escape-characters)
18. [Comments](#comments)
19. [Definition Lists](#definition-lists)
20. [Footnotes](#footnotes)

---

## Headings

### Heading 1 Syntax
```
# Heading 1
```

### Heading 2 Syntax
```
## Heading 2
```

### Heading 3 Syntax
```
### Heading 3
```

### Heading 4 Syntax
```
#### Heading 4
```

### Heading 5 Syntax
```
##### Heading 5
```

### Heading 6 Syntax
```
###### Heading 6
```

### Alternative Heading 1 Syntax
```
Heading 1
=========
```

### Alternative Heading 2 Syntax
```
Heading 2
---------
```

**Note:** The hash method is more commonly used. Headings must have a space between the hash(es) and the text.

---

## Paragraphs and Line Breaks

### Paragraph Syntax
```
This is a paragraph.
It can span multiple lines.

This is a new paragraph because there's a blank line above.
```

This is a paragraph.
It can span multiple lines.

This is a new paragraph because there's a blank line above.

### Line Break Syntax (Two Spaces)
```
Line one  
Line two (note two spaces after line one)
```

Line one  
Line two (note two spaces after line one)

### Line Break Syntax (Backslash)
```
Line one\
Line two
```

Line one\
Line two

### Explicit Line Break (<br>)
```
Line one<br>
Line two
```

Line one<br>
Line two

---

## Text Formatting

### Bold Syntax
```
**Bold text**
__Bold text__
```

**Bold text**
__Bold text__

### Italic Syntax
```
*Italic text*
_Italic text_
```

*Italic text*
_Italic text_

### Bold and Italic Syntax
```
***Bold and italic***
___Bold and italic___
**_Bold and italic_**
__*Bold and italic*__
```

***Bold and italic***
___Bold and italic___
**_Bold and italic_**
__*Bold and italic*__

### Bold with Asterisks
```
**Bold**
```

**Bold**

### Italic with Underscores
```
_Italic_
```

_Italic_

### Combined Formatting
```
**This is _bold and italic_**
__This is *bold and italic*__
```

**This is _bold and italic_**
__This is *bold and italic*__

---

## Lists

### Unordered List Syntax (Hyphens)
```
- Item 1
- Item 2
- Item 3
```

- Item 1
- Item 2
- Item 3

### Unordered List Syntax (Asterisks)
```
* Item 1
* Item 2
* Item 3
```

* Item 1
* Item 2
* Item 3

### Unordered List Syntax (Plus Signs)
```
+ Item 1
+ Item 2
+ Item 3
```

+ Item 1
+ Item 2
+ Item 3

### Ordered List Syntax
```
1. First item
2. Second item
3. Third item
```

1. First item
2. Second item
3. Third item

### Ordered List with Same Numbers
```
1. First item
1. Second item
1. Third item
```

1. First item
1. Second item
1. Third item

### Mixed List (Nested)
```
1. First item
2. Second item
   - Nested item
   - Another nested item
3. Third item
   1. Numbered nested
   2. Another numbered nested
```

1. First item
2. Second item
   - Nested item
   - Another nested item
3. Third item
   1. Numbered nested
   2. Another numbered nested

### List with Multiple Paragraphs
```
- Item 1

  Paragraph under item 1

- Item 2

  Paragraph under item 2
```

- Item 1

  Paragraph under item 1

- Item 2

  Paragraph under item 2

### List with Code Blocks
```
1. Item with code

   ```python
   print("Hello")
   ```

2. Another item
```

1. Item with code

   ```python
   print("Hello")
   ```

2. Another item

### List with Blockquotes
```
- Item 1
  > Quoted text
- Item 2
```

- Item 1
  > Quoted text
- Item 2

### Deeply Nested Lists
```
- Item 1
  - Nested 1
    - Double nested 1
      - Triple nested 1
```

- Item 1
  - Nested 1
    - Double nested 1
      - Triple nested 1

---

## Links

### Basic Link Syntax
```
[Link text](https://example.com)
```

[Link text](https://example.com)

### Link with Title
```
[Link text](https://example.com "Link title")
```

[Link text](https://example.com "Link title")

### Link with Parentheses in URL
```
[Link text](https://example.com/path(with)parentheses)
```

[Link text](https://example.com/path(with)parentheses)

### Automatic Link
```
<https://example.com>
```

<https://example.com>

### Email Link
```
<user@example.com>
```

<user@example.com>

### Reference Link
```
[Link text][ref]

[ref]: https://example.com
```

[Link text][ref]

[ref]: https://example.com

### Reference Link Short Form
```
[Link text]

[Link text]: https://example.com
```

[Link text]

[Link text]: https://example.com

### Link to Anchor/Heading
```
[Jump to Headings](#headings)
```

[Jump to Headings](#headings)

### Relative Links
```
[Local file](./path/to/file.md)
[Parent directory](../file.md)
```

### Link with Emphasis
```
**[Bold link](https://example.com)**
*[Italic link](https://example.com)*
```

**[Bold link](https://example.com)**
*[Italic link](https://example.com)*

### Link as Image
```
[![Alt text](image.jpg)](https://example.com)
```

---

## Images

### Basic Image Syntax
```
![Alt text](https://example.com/image.jpg)
```

![Alt text](https://via.placeholder.com/150)

### Image with Title
```
![Alt text](https://example.com/image.jpg "Image title")
```

![Alt text](https://via.placeholder.com/150 "Image title")

### Image with Width and Height (HTML)
```
<img src="https://example.com/image.jpg" width="200" height="100">
```

<img src="https://via.placeholder.com/150" width="200" height="100">

### Reference Image
```
![Alt text][img-ref]

[img-ref]: https://example.com/image.jpg
```

### Image Link
```
[![Alt text](image.jpg)](https://example.com)
```

### Image with Markdown Link
```
[Link with image](https://example.com)
![Image inside link](image.jpg)
```

### Centered Image (HTML)
```
<center>
  ![Alt text](image.jpg)
</center>
```

---

## Code

### Inline Code Syntax
```
This is `inline code` in a sentence.
```

This is `inline code` in a sentence.

### Code Block Syntax (Backticks)
```
```
code here
```
```

```
code here
```

### Code Block Syntax (Indented)
```
    code indented by 4 spaces
```

    code indented by 4 spaces

### Fenced Code Block with Language
````
```python
def hello():
    print("Hello, World!")
```
````

```python
def hello():
    print("Hello, World!")
```

### JavaScript Code Block
````
```javascript
const greeting = "Hello";
console.log(greeting);
```
````

```javascript
const greeting = "Hello";
console.log(greeting);
```

### Bash/Shell Code Block
````
```bash
#!/bin/bash
echo "Hello, World!"
```
````

```bash
#!/bin/bash
echo "Hello, World!"
```

### JSON Code Block
````
```json
{
  "name": "John",
  "age": 30
}
```
````

```json
{
  "name": "John",
  "age": 30
}
```

### HTML Code Block
````
```html
<div class="container">
  <p>Hello</p>
</div>
```
````

```html
<div class="container">
  <p>Hello</p>
</div>
```

### CSS Code Block
````
```css
.container {
  width: 100%;
  padding: 20px;
}
```
````

```css
.container {
  width: 100%;
  padding: 20px;
}
```

### SQL Code Block
````
```sql
SELECT * FROM users WHERE id = 1;
```
````

```sql
SELECT * FROM users WHERE id = 1;
```

### XML Code Block
````
```xml
<?xml version="1.0"?>
<root>
  <item>Value</item>
</root>
```
````

```xml
<?xml version="1.0"?>
<root>
  <item>Value</item>
</root>
```

### Plain Text Code Block
````
```plaintext
This is plain text
```
````

```plaintext
This is plain text
```

### Code Block with Line Numbers (GitHub Extensions)
````
```python
def hello():
    print("Hello")
```
````

### Syntax Highlighting with Different Languages
- `javascript`, `js`
- `python`, `py`
- `java`
- `csharp`, `cs`
- `cpp`, `c++`
- `c`
- `php`
- `ruby`, `rb`
- `go`, `golang`
- `rust`
- `swift`
- `kotlin`
- `typescript`, `ts`
- `html`, `xml`
- `css`, `scss`, `sass`
- `markdown`, `md`
- `bash`, `sh`, `zsh`
- `powershell`, `ps`, `ps1`
- `sql`
- `json`
- `yaml`, `yml`
- `toml`
- `ini`, `cfg`
- `diff`
- `tex`, `latex`

---

## Blockquotes

### Basic Blockquote
```
> This is a blockquote.
```

> This is a blockquote.

### Multi-line Blockquote
```
> This is a blockquote.
> It continues on the next line.
> And another line.
```

> This is a blockquote.
> It continues on the next line.
> And another line.

### Blockquote without repeating >
```
> This is a blockquote.
It continues without the >.
And another line.
```

> This is a blockquote.
It continues without the >.
And another line.

### Nested Blockquote
```
> This is a blockquote.
> 
> > This is a nested blockquote.
```

> This is a blockquote.
> 
> > This is a nested blockquote.

### Blockquote with Multiple Blocks
```
> This is a blockquote.
>
> - List item 1
> - List item 2
```

> This is a blockquote.
>
> - List item 1
> - List item 2

### Blockquote with Code Block
```
> ```python
> print("Code in blockquote")
> ```
```

> ```python
> print("Code in blockquote")
> ```

### Blockquote with Heading
```
> ## Heading in blockquote
> 
> Some text here.
```

> ## Heading in blockquote
> 
> Some text here.

### Blockquote with Formatted Text
```
> **Bold text** in blockquote
> *Italic text* in blockquote
> ***Bold and italic*** in blockquote
```

> **Bold text** in blockquote
> *Italic text* in blockquote
> ***Bold and italic*** in blockquote

---

## Horizontal Rules

### Horizontal Rule with Hyphens
```
---
```

---

### Horizontal Rule with Asterisks
```
***
```

***

### Horizontal Rule with Underscores
```
___
```

___

### Horizontal Rule with Many Hyphens
```
----
-----
------
```

----
-----
------

### Horizontal Rule with Spaces
```
- - -
* * *
_ _ _
```

---

## Tables

### Basic Table
```
| Header 1 | Header 2 |
|----------|----------|
| Cell 1   | Cell 2   |
| Cell 3   | Cell 4   |
```

| Header 1 | Header 2 |
|----------|----------|
| Cell 1   | Cell 2   |
| Cell 3   | Cell 4   |

### Table with Alignment
```
| Left | Center | Right |
|:-----|:------:|------:|
| L1   |   C1   |    R1 |
| L2   |   C2   |    R2 |
```

| Left | Center | Right |
|:-----|:------:|------:|
| L1   |   C1   |    R1 |
| L2   |   C2   |    R2 |

### Table with Multiple Columns
```
| Col 1 | Col 2 | Col 3 | Col 4 |
|-------|-------|-------|-------|
| A     | B     | C     | D     |
| E     | F     | G     | H     |
```

| Col 1 | Col 2 | Col 3 | Col 4 |
|-------|-------|-------|-------|
| A     | B     | C     | D     |
| E     | F     | G     | H     |

### Table with Formatted Content
```
| Feature | **Enabled** | Status |
|---------|-------------|--------|
| *Bold*  | Yes         | ✓      |
| _Italic_ | No         | ✗      |
```

| Feature | **Enabled** | Status |
|---------|-------------|--------|
| *Bold*  | Yes         | ✓      |
| _Italic_ | No         | ✗      |

### Table with Code
```
| Function | Description |
|----------|-------------|
| `func()` | Does something |
| `other()`| Does other |
```

| Function | Description |
|----------|-------------|
| `func()` | Does something |
| `other()`| Does other |

### Table with Links
```
| Name | Link |
|------|------|
| Google | [Visit](https://google.com) |
| GitHub | [Visit](https://github.com) |
```

| Name | Link |
|------|------|
| Google | [Visit](https://google.com) |
| GitHub | [Visit](https://github.com) |

### Table with Images
```
| Icon | Name |
|------|------|
| ![](https://via.placeholder.com/20) | Item 1 |
| ![](https://via.placeholder.com/20) | Item 2 |
```

| Icon | Name |
|------|------|
| ![](https://via.placeholder.com/20) | Item 1 |
| ![](https://via.placeholder.com/20) | Item 2 |

### Alignment Markers Explained
```
| Left | Center | Right |
|:-----|:------:|------:|
```

- `|:---` = Left aligned
- `|:---:` = Center aligned
- `---:|` = Right aligned
- `|---` = Default (left aligned)

### Table without Outer Pipes
```
Header 1 | Header 2
---------|----------
Cell 1   | Cell 2
Cell 3   | Cell 4
```

Header 1 | Header 2
---------|----------
Cell 1   | Cell 2
Cell 3   | Cell 4

---

## Task Lists

### Basic Task List
```
- [x] Completed task
- [ ] Incomplete task
- [x] Another completed task
```

- [x] Completed task
- [ ] Incomplete task
- [x] Another completed task

### Task List with Nesting
```
- [x] Parent task
  - [x] Subtask 1
  - [ ] Subtask 2
- [ ] Another parent task
  - [ ] Subtask 3
```

- [x] Parent task
  - [x] Subtask 1
  - [ ] Subtask 2
- [ ] Another parent task
  - [ ] Subtask 3

### Ordered Task List
```
1. [x] First task
2. [ ] Second task
3. [x] Third task
```

1. [x] First task
2. [ ] Second task
3. [x] Third task

---

## Strikethrough

### Basic Strikethrough
```
~~Strikethrough text~~
```

~~Strikethrough text~~

### Strikethrough with Other Formatting
```
~~**Bold strikethrough**~~
~~*Italic strikethrough*~~
```

~~**Bold strikethrough**~~
~~*Italic strikethrough*~~

---

## Subscript and Superscript

### Subscript (HTML)
```
H<sub>2</sub>O
```

H<sub>2</sub>O

### Superscript (HTML)
```
E=mc<sup>2</sup>
```

E=mc<sup>2</sup>

### Superscript with Caret (Some Markdown)
```
This is superscript: x^2^
```

This is superscript: x^2^

### Subscript with Tilde (Some Markdown)
```
This is subscript: H~2~O
```

This is subscript: H~2~O

---

## Highlighting

### Highlight with HTML Mark Tag
```
This is <mark>highlighted</mark> text.
```

This is <mark>highlighted</mark> text.

### Highlight with Background Color (HTML)
```
<span style="background-color: yellow">Highlighted</span>
```

<span style="background-color: yellow">Highlighted</span>

### Highlight with Multiple Colors
```
<span style="background-color: #FFFF00">Yellow</span>
<span style="background-color: #00FF00">Green</span>
<span style="background-color: #FF0000">Red</span>
```

<span style="background-color: #FFFF00">Yellow</span>
<span style="background-color: #00FF00">Green</span>
<span style="background-color: #FF0000">Red</span>

---

## Emojis

### Emoji Unicode
```
😀 😁 😂 🤣 😃 😄 😅
🎉 🎊 🎈 🎁 🎀
❤️ 💔 💕 💖 💗
👍 👎 👏 🙏 ✋
```

😀 😁 😂 🤣 😃 😄 😅
🎉 🎊 🎈 🎁 🎀
❤️ 💔 💕 💖 💗
👍 👎 👏 🙏 ✋

### Emoji Codes (GitHub)
```
:smile: :laughing: :blush: :grinning:
:+1: :-1: :clap: :fire: :tada:
:heart: :star: :star2: :sparkles:
```

:smile: :laughing: :blush: :grinning:
:+1: :-1: :clap: :fire: :tada:
:heart: :star: :star2: :sparkles:

---

## HTML Elements

### HTML Div
```
<div style="color: red;">
  This text is red.
</div>
```

<div style="color: red;">
  This text is red.
</div>

### HTML Span
```
This is <span style="color: blue;">blue text</span> in a sentence.
```

This is <span style="color: blue;">blue text</span> in a sentence.

### HTML Bold
```
<b>Bold text</b>
```

<b>Bold text</b>

### HTML Italic
```
<i>Italic text</i>
```

<i>Italic text</i>

### HTML Underline
```
<u>Underlined text</u>
```

<u>Underlined text</u>

### HTML Small
```
<small>Small text</small>
```

<small>Small text</small>

### HTML Paragraph
```
<p>This is a paragraph.</p>
```

<p>This is a paragraph.</p>

### HTML Heading
```
<h1>HTML Heading 1</h1>
<h2>HTML Heading 2</h2>
```

<h1>HTML Heading 1</h1>
<h2>HTML Heading 2</h2>

### HTML Line Break
```
Line 1<br>Line 2
```

Line 1<br>Line 2

### HTML Horizontal Rule
```
<hr>
```

<hr>

### HTML Comment
```
<!-- This is a comment and won't be displayed -->
```

<!-- This is a comment and won't be displayed -->

### HTML Table
```
<table>
  <tr>
    <th>Header 1</th>
    <th>Header 2</th>
  </tr>
  <tr>
    <td>Cell 1</td>
    <td>Cell 2</td>
  </tr>
</table>
```

<table>
  <tr>
    <th>Header 1</th>
    <th>Header 2</th>
  </tr>
  <tr>
    <td>Cell 1</td>
    <td>Cell 2</td>
  </tr>
</table>

### HTML List
```
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
</ul>
```

<ul>
  <li>Item 1</li>
  <li>Item 2</li>
</ul>

### HTML Button
```
<button onclick="alert('Hello!')">Click Me</button>
```

<button onclick="alert('Hello!')">Click Me</button>

### HTML Input
```
<input type="text" placeholder="Enter text">
```

<input type="text" placeholder="Enter text">

### HTML Details/Summary
```
<details>
  <summary>Click to expand</summary>
  Hidden content here
</details>
```

<details>
  <summary>Click to expand</summary>
  Hidden content here
</details>

### HTML Form
```
<form>
  <label>Name:</label><br>
  <input type="text"><br>
  <label>Email:</label><br>
  <input type="email"><br>
  <button type="submit">Submit</button>
</form>
```

<form>
  <label>Name:</label><br>
  <input type="text"><br>
  <label>Email:</label><br>
  <input type="email"><br>
  <button type="submit">Submit</button>
</form>

---

## Escape Characters

### Escaping Markdown Syntax
```
\*Not italic\*
\[Not a link\]
\`Not code\`
\# Not a heading
\- Not a list item
```

\*Not italic\*
\[Not a link\]
\`Not code\`
\# Not a heading
\- Not a list item

### All Escapable Characters
```
\\ backslash
\` backtick
\* asterisk
\_ underscore
\{ } curly braces
\[ ] square brackets
\( ) parentheses
\# hash
\+ plus
\- minus/hyphen
\. period
\! exclamation mark
\| pipe
```

\\ backslash
\` backtick
\* asterisk
\_ underscore
\{ } curly braces
\[ ] square brackets
\( ) parentheses
\# hash
\+ plus
\- minus/hyphen
\. period
\! exclamation mark
\| pipe

---

## Comments

### HTML Comment (Hidden)
```
<!-- This is a comment -->
```

<!-- This is a comment -->

### Multi-line HTML Comment
```
<!--
This is a multi-line comment.
It won't be displayed.
Even with multiple paragraphs.
-->
```

<!--
This is a multi-line comment.
It won't be displayed.
Even with multiple paragraphs.
-->

### Comment with Content After
```
<!-- Comment here -->
This text will be shown.
```

<!-- Comment here -->
This text will be shown.

---

## Definition Lists

### Basic Definition List (HTML)
```
<dl>
  <dt>Term 1</dt>
  <dd>Definition of term 1</dd>
  <dt>Term 2</dt>
  <dd>Definition of term 2</dd>
</dl>
```

<dl>
  <dt>Term 1</dt>
  <dd>Definition of term 1</dd>
  <dt>Term 2</dt>
  <dd>Definition of term 2</dd>
</dl>

### Definition List with Multiple Definitions
```
<dl>
  <dt>Term</dt>
  <dd>First definition</dd>
  <dd>Second definition</dd>
</dl>
```

<dl>
  <dt>Term</dt>
  <dd>First definition</dd>
  <dd>Second definition</dd>
</dl>

---

## Footnotes

### Basic Footnote
```
This is text with a footnote[^1].

[^1]: This is the footnote explanation.
```

This is text with a footnote[^1].

[^1]: This is the footnote explanation.

### Multiple Footnotes
```
First footnote[^1] and second[^2].

[^1]: First explanation.
[^2]: Second explanation.
```

First footnote[^1] and second[^2].

[^1]: First explanation.
[^2]: Second explanation.

### Named Footnotes
```
Reference[^note].

[^note]: This is a named footnote.
```

Reference[^note].

[^note]: This is a named footnote.

### Footnote with Multiple Paragraphs
```
Text with footnote[^complex].

[^complex]: First paragraph.

    Second paragraph in footnote.
```

Text with footnote[^complex].

[^complex]: First paragraph.

    Second paragraph in footnote.

---

## Advanced Combinations

### Heading with Formatting
```
## This is **bold** and *italic* heading
```

## This is **bold** and *italic* heading

### Paragraph with Multiple Formatting
```
This paragraph has **bold**, *italic*, ***bold italic***, `code`, ~~strikethrough~~, and [links](https://example.com).
```

This paragraph has **bold**, *italic*, ***bold italic***, `code`, ~~strikethrough~~, and [links](https://example.com).

### List with Multiple Formatting
```
- **Bold item**
- *Italic item*
- `Code item`
- [Link item](https://example.com)
- ~~Strikethrough item~~
```

- **Bold item**
- *Italic item*
- `Code item`
- [Link item](https://example.com)
- ~~Strikethrough item~~

### Complex Blockquote
```
> ## Heading in quote
> 
> This is **bold** and *italic* text.
> 
> ```python
> code_in_quote = True
> ```
> 
> - List item 1
> - List item 2
```

> ## Heading in quote
> 
> This is **bold** and *italic* text.
> 
> ```python
> code_in_quote = True
> ```
> 
> - List item 1
> - List item 2

### Table in List
```
- Item 1
  | Col 1 | Col 2 |
  |-------|-------|
  | A     | B     |

- Item 2
```

---

## Special Markdown Extensions

### Abbreviations
```
The HTML specification is maintained by the W3C.

*[HTML]: Hyper Text Markup Language
*[W3C]: World Wide Web Consortium
```

### Footnote with Link
```
See this[^1] source.

[^1]: [https://example.com](https://example.com)
```

### Keyboard Input (HTML)
```
Press <kbd>Ctrl</kbd> + <kbd>C</kbd> to copy.
```

Press <kbd>Ctrl</kbd> + <kbd>C</kbd> to copy.

### Variable (HTML)
```
The formula is <var>a</var> + <var>b</var> = <var>c</var>
```

The formula is <var>a</var> + <var>b</var> = <var>c</var>

### Code Output (HTML)
```
<samp>Output: Success</samp>
```

<samp>Output: Success</samp>

### Math LaTeX (Some Markdown)
```
$$E = mc^2$$
$$\sum_{i=1}^{n} i = \frac{n(n+1)}{2}$$
```

Inline math: $a^2 + b^2 = c^2$

### Directory Tree (Code Block)
```
.
├── src/
│   ├── main.js
│   └── utils.js
├── tests/
│   └── test.js
└── README.md
```

---

## Markdown Syntax Cheat Sheet

| Element | Markdown Syntax |
|---------|-----------------|
| Heading 1 | `# Heading 1` |
| Heading 2 | `## Heading 2` |
| Bold | `**bold**` or `__bold__` |
| Italic | `*italic*` or `_italic_` |
| Code | `` `code` `` |
| Code Block | ` ```code block``` ` |
| Link | `[text](url)` |
| Image | `![alt](url)` |
| Blockquote | `> quote` |
| List | `- item` or `1. item` |
| Horizontal Rule | `---` |
| Strikethrough | `~~text~~` |
| Table | See Tables section |
| Task List | `- [x] task` |

---

## Tips and Best Practices

1. **Consistency**: Use the same symbols for lists (hyphens, asterisks, or plus signs) throughout your document.

2. **Spacing**: Always add blank lines between different block elements for proper rendering.

3. **Code Blocks**: Always specify the language for better syntax highlighting.

4. **Tables**: Use tools to generate table markdown to avoid errors.

5. **Links**: Use descriptive link text instead of "click here".

6. **Line Breaks**: Prefer blank lines over two spaces or backslashes.

7. **Readability**: Format your markdown source for readability, not just the output.

8. **Nesting**: When nesting lists or blockquotes, use consistent indentation (typically 2 or 4 spaces).

9. **HTML**: Only use HTML when standard Markdown doesn't provide the needed functionality.

10. **Escape Characters**: Use backslash escapes when you need to display special characters literally.

---

## Markdown Flavors

Different Markdown implementations may support different extensions:

- **CommonMark**: Standard Markdown specification
- **GitHub Flavored Markdown (GFM)**: Adds tables, task lists, strikethrough
- **MultiMarkdown**: Adds footnotes, citations, metadata
- **Markdown Extra**: Adds definition lists, abbreviations, footnotes
- **kramdown**: Used by Jekyll, adds block attributes and more
- **Pandoc Markdown**: Powerful and flexible with many extensions

---

## Conclusion

This comprehensive guide covers all standard Markdown syntax and many extensions. Practice using these elements to create well-formatted, readable documents. Remember that while HTML can provide more control, Markdown's simplicity and readability are its greatest strengths.