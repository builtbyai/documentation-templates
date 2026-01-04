# Advanced Markdown Template

**Purpose**: Advanced markdown syntax and formatting techniques
**Source**: Compiled from 6 Obsidian vault templates
**Usage**: Master advanced markdown features for professional documentation

---

## Table of Contents
1. [Tables with Styling](#tables-with-styling)
2. [Anchor Links & TOC](#anchor-links--toc)
3. [Blockquotes & Citations](#blockquotes--citations)
4. [Lists & Nesting](#lists--nesting)
5. [Code Blocks](#code-blocks)
6. [Horizontal Rules](#horizontal-rules)
7. [Text Formatting](#text-formatting)

---

## Tables with Styling

### Basic Table
```markdown
| Column 1 | Column 2 | Column 3 |
|----------|----------|----------|
| Row 1, Col 1 | Row 1, Col 2 | Row 1, Col 3 |
| Row 2, Col 1 | Row 2, Col 2 | Row 2, Col 3 |
```

**Result**:
| Column 1 | Column 2 | Column 3 |
|----------|----------|----------|
| Row 1, Col 1 | Row 1, Col 2 | Row 1, Col 3 |
| Row 2, Col 1 | Row 2, Col 2 | Row 2, Col 3 |

### Table with Alignment
```markdown
| Left Aligned | Center Aligned | Right Aligned |
|:-------------|:--------------:|--------------:|
| Text         | Text           | Text          |
| More text    | More text      | More text     |
```

**Result**:
| Left Aligned | Center Aligned | Right Aligned |
|:-------------|:--------------:|--------------:|
| Text         | Text           | Text          |
| More text    | More text      | More text     |

### Table with Emojis and Styling
```markdown
| Status | Feature | Priority | Progress |
|:------:|---------|:--------:|:--------:|
| ✅ | User Authentication | 🔴 High | 100% |
| ⏳ | Dashboard Analytics | 🟠 Medium | 75% |
| ❌ | Email Notifications | 🟢 Low | 0% |
| ✅ | API Integration | 🟠 Medium | 100% |
```

**Result**:
| Status | Feature | Priority | Progress |
|:------:|---------|:--------:|:--------:|
| ✅ | User Authentication | 🔴 High | 100% |
| ⏳ | Dashboard Analytics | 🟠 Medium | 75% |
| ❌ | Email Notifications | 🟢 Low | 0% |
| ✅ | API Integration | 🟠 Medium | 100% |

### Comparison Table
```markdown
| Feature | Basic Plan | Pro Plan | Enterprise |
|---------|:----------:|:--------:|:----------:|
| Users | 5 | 50 | Unlimited |
| Storage | 10 GB | 100 GB | 1 TB |
| Support | Email | Email + Chat | 24/7 Phone |
| Price | $9/mo | $29/mo | Custom |
| **Value** | ⭐⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ |
```

**Result**:
| Feature | Basic Plan | Pro Plan | Enterprise |
|---------|:----------:|:--------:|:----------:|
| Users | 5 | 50 | Unlimited |
| Storage | 10 GB | 100 GB | 1 TB |
| Support | Email | Email + Chat | 24/7 Phone |
| Price | $9/mo | $29/mo | Custom |
| **Value** | ⭐⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ |

---

## Anchor Links & TOC

### Creating Anchors
```markdown
## Section Name {#custom-anchor}

Content here...

[Jump to Section Name](#custom-anchor)
```

### Auto-Generated TOC
```markdown
## Table of Contents
- [Introduction](#introduction)
- [Getting Started](#getting-started)
  - [Installation](#installation)
  - [Configuration](#configuration)
- [Usage](#usage)
- [API Reference](#api-reference)
- [FAQ](#faq)

## Introduction
Content...

## Getting Started
Content...

### Installation
Content...

### Configuration
Content...
```

### Internal Document Links
```markdown
See [Advanced Usage](#advanced-usage) for more details.

For troubleshooting, check the [FAQ section](#faq).

Refer to [Configuration Options](#configuration-options) to customize settings.
```

---

## Blockquotes & Citations

### Simple Blockquote
```markdown
> This is a simple blockquote.
> It can span multiple lines.
```

**Result**:
> This is a simple blockquote.
> It can span multiple lines.

### Nested Blockquotes
```markdown
> First level quote
>
> > Nested quote
> >
> > > Deep nested quote
>
> Back to first level
```

**Result**:
> First level quote
>
> > Nested quote
> >
> > > Deep nested quote
>
> Back to first level

### Quote with Attribution
```markdown
> "The best way to predict the future is to invent it."
>
> — Alan Kay
```

**Result**:
> "The best way to predict the future is to invent it."
>
> — Alan Kay

### Multi-Paragraph Blockquote
```markdown
> This is the first paragraph of a longer quote.
>
> This is the second paragraph, still within the same quote block.
> Notice the blank line with just `>` to separate paragraphs.
>
> Final paragraph with more content.
```

**Result**:
> This is the first paragraph of a longer quote.
>
> This is the second paragraph, still within the same quote block.
> Notice the blank line with just `>` to separate paragraphs.
>
> Final paragraph with more content.

### Blockquote with Code
```markdown
> Code example within a quote:
>
> ```javascript
> function example() {
>   return "This is code inside a blockquote";
> }
> ```
```

---

## Lists & Nesting

### Unordered Lists
```markdown
- Item 1
- Item 2
- Item 3
  - Nested item 3.1
  - Nested item 3.2
    - Deeply nested item 3.2.1
- Item 4
```

**Result**:
- Item 1
- Item 2
- Item 3
  - Nested item 3.1
  - Nested item 3.2
    - Deeply nested item 3.2.1
- Item 4

### Ordered Lists
```markdown
1. First item
2. Second item
3. Third item
   1. Nested numbered item
   2. Another nested item
      1. Deeply nested
4. Fourth item
```

**Result**:
1. First item
2. Second item
3. Third item
   1. Nested numbered item
   2. Another nested item
      1. Deeply nested
4. Fourth item

### Mixed Lists
```markdown
1. Ordered item
2. Another ordered item
   - Unordered nested item
   - Another unordered nested item
     1. Back to ordered
     2. Still ordered
3. Back to main ordered list
   - Mix it up again
```

**Result**:
1. Ordered item
2. Another ordered item
   - Unordered nested item
   - Another unordered nested item
     1. Back to ordered
     2. Still ordered
3. Back to main ordered list
   - Mix it up again

### Lists with Paragraphs
```markdown
1. First item with multiple paragraphs

   This is the second paragraph of the first item.
   Notice the blank line above.

2. Second item

   With another paragraph here.

3. Third item
```

### Definition Lists (Extended Markdown)
```markdown
Term 1
: Definition of term 1

Term 2
: Definition of term 2
: Another definition of term 2

Term 3
: Definition with multiple paragraphs

  Second paragraph of definition
```

---

## Code Blocks

### Inline Code
```markdown
Use `console.log()` to print output.
The variable `userName` stores the user's name.
```

**Result**:
Use `console.log()` to print output.
The variable `userName` stores the user's name.

### Code Blocks with Syntax Highlighting

**JavaScript**:
````markdown
```javascript
function greet(name) {
  console.log(`Hello, ${name}!`);
}

greet("World");
```
````

**Python**:
````markdown
```python
def calculate_sum(a, b):
    """Calculate sum of two numbers"""
    return a + b

result = calculate_sum(5, 3)
print(f"Result: {result}")
```
````

**HTML**:
````markdown
```html
<!DOCTYPE html>
<html>
<head>
    <title>Page Title</title>
</head>
<body>
    <h1>Hello World</h1>
</body>
</html>
```
````

**CSS**:
````markdown
```css
.container {
    display: flex;
    justify-content: center;
    align-items: center;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
}
```
````

**JSON**:
````markdown
```json
{
  "name": "John Doe",
  "age": 30,
  "email": "john@example.com",
  "roles": ["admin", "user"]
}
```
````

**Shell/Bash**:
````markdown
```bash
#!/bin/bash

# Install dependencies
npm install

# Run tests
npm test

# Build project
npm run build
```
````

### Code Block with Line Numbers (Plugin-Dependent)
````markdown
```javascript {numberLines}
function fibonacci(n) {
  if (n <= 1) return n;
  return fibonacci(n - 1) + fibonacci(n - 2);
}

console.log(fibonacci(10));
```
````

### Code Block with Highlighting (Plugin-Dependent)
````markdown
```javascript {3-5}
function example() {
  const data = fetchData();
  const processed = process(data);  // highlighted
  const validated = validate(processed);  // highlighted
  return validated;  // highlighted
}
```
````

---

## Horizontal Rules

### Different Styles
```markdown
Method 1: Three hyphens
---

Method 2: Three asterisks
***

Method 3: Three underscores
___
```

**Result**:
---

### Using as Section Dividers
```markdown
## Section One

Content for section one...

---

## Section Two

Content for section two...

---

## Section Three

Content for section three...
```

---

## Text Formatting

### Basic Formatting
```markdown
**Bold text** or __bold text__
*Italic text* or _italic text_
***Bold and italic*** or ___bold and italic___
~~Strikethrough text~~
`Inline code`
```

**Result**:
**Bold text** or __bold text__
*Italic text* or _italic text_
***Bold and italic*** or ___bold and italic___
~~Strikethrough text~~
`Inline code`

### Headings
```markdown
# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6
```

**Result**:
# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6

### Alternate Heading Syntax
```markdown
Heading 1
=========

Heading 2
---------
```

### Subscript and Superscript (Extended Markdown)
```markdown
H~2~O (subscript - plugin dependent)
x^2^ (superscript - plugin dependent)

Alternative HTML:
H<sub>2</sub>O
E = mc<sup>2</sup>
```

**Result**:
H<sub>2</sub>O
E = mc<sup>2</sup>

### Highlighting (Plugin-Dependent)
```markdown
==Highlighted text==
<mark>Highlighted using HTML</mark>
```

### Links
```markdown
[Link text](https://example.com)
[Link with title](https://example.com "Hover text here")
<https://example.com>
<email@example.com>

Reference-style links:
[Link text][reference]

[reference]: https://example.com "Optional title"
```

### Images
```markdown
![Alt text](image.png)
![Alt text](image.png "Optional title")

With link:
[![Alt text](image.png)](https://example.com)

Reference-style:
![Alt text][image-ref]

[image-ref]: image.png "Optional title"
```

### Footnotes (Extended Markdown)
```markdown
Here is a sentence with a footnote.[^1]

[^1]: This is the footnote content.

Another footnote reference.[^note]

[^note]: Footnotes can have any identifier.
```

### Keyboard Keys (HTML)
```html
Press <kbd>Ctrl</kbd> + <kbd>C</kbd> to copy
Press <kbd>⌘</kbd> + <kbd>V</kbd> to paste
```

**Result**:
Press <kbd>Ctrl</kbd> + <kbd>C</kbd> to copy
Press <kbd>⌘</kbd> + <kbd>V</kbd> to paste

### Task Lists (GitHub Flavored Markdown)
```markdown
- [x] Completed task
- [ ] Incomplete task
- [x] Another completed task
```

**Result**:
- [x] Completed task
- [ ] Incomplete task
- [x] Another completed task

---

## Advanced Techniques

### Escaping Characters
```markdown
Use backslash to escape special characters:
\* Not italic \*
\# Not a heading
\[Not a link](url)
\`Not code\`
```

### HTML in Markdown
```markdown
You can use HTML directly:

<div style="background: #f0f0f0; padding: 20px; border-radius: 8px;">
    <strong>HTML content</strong> mixed with <em>markdown</em>
</div>

<details>
<summary>Click to expand</summary>

This content is hidden by default!

</details>
```

### Line Breaks
```markdown
Method 1: Two spaces at end of line
Next line

Method 2: Backslash at end\
Next line

Method 3: <br> HTML tag<br>
Next line
```

### Comments (HTML)
```markdown
<!-- This is a comment and won't be visible -->

Visible text here
<!-- Another hidden comment -->
More visible text
```

### Emoji (Plugin/Platform-Dependent)
```markdown
:smile: :heart: :thumbsup: :rocket: :fire:

Or use Unicode directly:
😊 ❤️ 👍 🚀 🔥
```

### Math Equations (LaTeX - Plugin-Dependent)
````markdown
Inline math: $E = mc^2$

Block math:
$$
\frac{-b \pm \sqrt{b^2 - 4ac}}{2a}
$$
````

---

## Best Practices

### Formatting Guidelines
1. **Consistent Heading Hierarchy**: Don't skip levels (H1 → H2 → H3, not H1 → H3)
2. **Blank Lines**: Add blank lines before and after headings, code blocks, lists
3. **List Indentation**: Use 2-4 spaces for nested lists (be consistent)
4. **Code Language**: Always specify language for syntax highlighting
5. **Link References**: Use reference-style for frequently used links

### Readability Tips
- **Chunk Content**: Break long content into sections with headers
- **Use Lists**: Lists are easier to scan than paragraphs
- **Highlight Key Points**: Use bold or tables for important information
- **Add TOC**: Include table of contents for long documents
- **Code Examples**: Provide complete, runnable examples when possible

### Organization
```markdown
# Document Title

> Brief description or abstract

## Table of Contents
- [Section 1](#section-1)
- [Section 2](#section-2)

---

## Section 1

Content...

### Subsection 1.1

Content...

---

## Section 2

Content...

---

## References

- [Link 1](url)
- [Link 2](url)
```

---

## Markdown Variants

### GitHub Flavored Markdown (GFM)
- Task lists: `- [ ]` and `- [x]`
- Tables with alignment
- Strikethrough: `~~text~~`
- Automatic URL linking
- Username mentions: `@username`
- Issue references: `#123`
- Emoji shortcodes: `:emoji:`

### Obsidian Markdown
- Wiki-style links: `[[Page Name]]`
- Callouts: `> [!info]`
- Embedded files: `![[file.pdf]]`
- Tags: `#tag`
- Math: `$equation$`

### CommonMark
- Strict standard specification
- Predictable parsing
- Most compatible across platforms

---

**Template Version**: 1.0
**Last Updated**: 2025-12-28
**Markdown Flavor**: Universal (compatible with CommonMark, GFM, Obsidian)
**Source Files**: 6 Obsidian markdown templates
