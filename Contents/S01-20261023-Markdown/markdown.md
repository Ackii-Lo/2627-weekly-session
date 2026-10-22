---
marp: true
theme: cpu
paginate: true
math: mathjax
---

<!-- _class: lead -->

<style scoped>
section.lead img {
  position: absolute;
  left: 84px;
  bottom: 58px;
  width: 140px;
  height: auto;
}
</style>

# A Quick Introduction to Markdown
## 

Computer Psycho Union - Markdown

23 October 2026

![w:140](./assets/software-icons/markdown.png)
### Markdown

#### CPU

---

<!-- _class: agenda -->

## Agenda

1. Markdown Overview  *origins, tools, and use cases*
2. Text Structure and Lists  *headings, paragraphs, and lists*
3. Common Formatting  *emphasis, links, quotations, and formulas*
4. Practice & Review  *an introduction card, review, and application*

---

<!-- _class: yellow -->

## PART 01

### 01

#### Markdown Overview

Let's get to know Markdown

---

## 01 - Where Did Markdown Come From?

Markdown was introduced in 2004 by **John Gruber** for people who write for the web. It began as a lightweight way to turn plain text into HTML: people write text that is easy to read, and tools turn it into structured web content.

Its design was inspired by plain-text email. Even before conversion, headings, lists, and links should remain broadly understandable. That readability is why Markdown still works so well for notes and documents today.

- **John Gruber** published the early implementation and syntax description
- **Aaron Swartz** contributed important ideas, feedback, and testing to the format's design
- "Readability first" remains Markdown's most important design principle


*Source: Daring Fireball - Markdown (2004)*

---

## 02 - What Is Markdown, and Why Use It?

Markdown is a lightweight markup language. It uses a small number of symbols to represent structure such as headings, lists, and links. A `.md` file can be opened in an ordinary editor and converted by different tools into web pages, notes, or documents.


Instead of repeatedly adjusting font size and indentation in an interface, Markdown focuses on the hierarchy of the content itself. Write the structure clearly first, then let the tool handle the presentation.

> **Markdown is not meant to make writing more complicated. It keeps text simple, readable, and portable.**



---

## 03 - A Minimal Markdown File

These few lines already make a complete Markdown note:

```markdown
# My Weekend Plan

- Take a walk in Yinzhou Park
- Have McDonald's
```

`#` indicates a heading, and `-` starts an unordered list. Once the file is saved as `hello.md`, it remains a clear plain-text document even without specialised software.

---

## 04 - Where Can You Write Markdown?

Markdown is fundamentally a text-file format, so you can write it in many applications. Each tool has a different focus; choose one based on what you mainly need to do.

<style scoped>
.tool-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 14px 18px;
  margin: 18px 0 14px;
}
.tool-card {
  display: grid;
  grid-template-columns: 62px 1fr;
  align-items: center;
  min-height: 104px;
  padding: 12px 18px;
  border: 2.5px solid #111;
  box-shadow: 6px 6px 0 #f7d447;
  background: #fff;
}
.tool-card img {
  width: 46px;
  height: 46px;
  object-fit: contain;
  border-radius: 10px;
}
.tool-card strong {
  display: inline-block;
  margin-bottom: 3px;
  padding: 0 7px;
  background: #f7d447;
  font-size: 20px;
  line-height: 1.45;
}
.tool-card span {
  display: block;
  font-size: 17px;
  line-height: 1.45;
}
</style>

<div class="tool-grid">
  <div class="tool-card">
    <img src="assets/software-icons/vscode.png" alt="VS Code icon">
    <div><strong>VS Code</strong><span>Great for learning, project documentation, and file management</span></div>
  </div>
  <div class="tool-card">
    <img src="assets/software-icons/typora.png" alt="Typora icon">
    <div><strong>Typora</strong><span>Ideal for personal writing with a live formatted preview</span></div>
  </div>
  <div class="tool-card">
    <img src="assets/software-icons/obsidian.png" alt="Obsidian icon">
    <div><strong>Obsidian</strong><span>Useful for building a long-term personal knowledge base with links</span></div>
  </div>
  <div class="tool-card">
    <img src="assets/software-icons/github.svg" alt="GitHub icon">
    <div><strong>GitHub Web Editor</strong><span>Useful for editing documentation directly in an open-source project</span></div>
  </div>
</div>

Whichever tool you use, the syntax is the same. You do not need to rewrite your content when you switch tools.

---

## 05 - Markdown in Everyday Life and Projects

The most common example is the `README.md` file in the root directory of a GitHub repository. It usually explains what a project is, how to install and use it, and where to report problems.

- Course notes, lab records, and personal knowledge bases
- `README.md` files, contribution guides, and changelogs for open-source projects
- Technical blogs, online documentation, and team collaboration guides
- Methods, formulas, and result explanations in data-analysis reports

When you need others to understand content quickly, Markdown is often clearer than a large block of plain text.

---

## 06 - Using VS Code Today

In VS Code, create a file and save it as `hello.md` to start writing Markdown. The built-in preview updates as you edit, so no extra Markdown extension is required.

- macOS: `Cmd + Shift + V` opens the preview
- Windows / Linux: `Ctrl + Shift + V` opens the preview
- macOS: press `Cmd + K`, then `V`, to open a side-by-side preview
- Windows / Linux: press `Ctrl + K`, then `V`, to open a side-by-side preview

One side shows the source file and the other shows what readers see. Viewing both at once is the fastest way to learn Markdown.
> An online editor is available for participants who have not installed VS Code: https://md.harleyblog.cn/
---

<!-- _class: activities -->

## Exercise 01 - Create Your First Markdown File

### Task

- Create a file named `hello.md`
- Type a heading beginning with `#`
- Write one thing you want to accomplish today beneath the heading

### Check

- Does the filename end in `.md`?
- Is there one space after `#`?
- Can a reader understand your heading at a glance?

---

<!-- _class: yellow -->

## PART 02

### 02

#### Text Structure and Lists

Establish the hierarchy first, then add the details

---

## 07 - Headings and Paragraphs

Headings show the hierarchy of content. The fewer `#` symbols you use, the higher the heading level. A short article usually begins with one level-one heading, then uses level-two and level-three headings to organise topics.

```markdown
# Level-one heading: the subject of the whole note
## Level-two heading: a main section
### Level-three heading: a point within that section
```

Leave one blank line between paragraphs. A normal line break usually does not begin a new paragraph; to force a line break within the same paragraph, leave two spaces at the end of the line.

---

<!-- _class: activities -->


## 08 - Lists and Steps

Use an unordered list when items have no fixed order; use an ordered list when their order cannot be changed. Lists turn a large paragraph into easy-to-scan points.

```markdown
- An unordered list
- Works well for listing your ideas

1. An ordered sequence
2. Works well for procedures
   - Indent a sub-item by three spaces
```

Unordered lists are useful for tasks, features, and materials. Ordered lists work well for procedures, timelines, and checklists.

---

<!-- _class: activities -->

## Exercise 02 - Headings, Paragraphs, and Lists

### Task

- Write `My Weekend` using `##`
- Write two sentences with one blank line between them
- Use `-` to list three things you would like to do
- Use `1.` to write a three-step weekend plan


---

<!-- _class: yellow -->

## PART 03

### 03

#### Common Formatting

Let's make our content richer

---

## 09 - Emphasis, Links, and Code

Inline formatting helps readers spot keywords, supplementary information, and filenames. It should make important content easier to find, rather than making the whole page stand out.

```markdown
**Important information**
*Supplementary note*
[Visit example](https://example.com)
`hello.md`
```

`**text**` highlights a key conclusion, `*text*` adds a supplementary note, `[label](URL)` creates a link, and backticks are commonly used for filenames, commands, and short code fragments.

---

## 10 - Quotations, Images, and Tables

Use `>` for a reminder, quotation, or conclusion that deserves separate attention. Insert an image with `![description](path)`; the description should tell readers what it conveys.
Tables compare a small amount of information side by side. For a simple vertical sequence, a list is usually clearer.

```markdown
| Tool | Best for |
| --- | --- |
| Markdown | Writing content |
| Text editor | Editing files |
```

---

## 11 - Horizontal Rules

A horizontal rule separates different topics or stages in a document. Enter three or more identical symbols on their own line to create one.

```text
Content above

Horizontal rule: --- (when writing it, keep only the three hyphens)

Content below
```

When you write one, keep only the symbols on the line. `---`, `***`, and `___` produce the same result.

- The symbols must occupy their own line
- Leave a blank line before and after the rule for a clearer structure
- Use rules between chapters or major topics; do not overuse them

---

<!-- _class: activities -->

## Exercise 03 - Choose the Right Form of Expression

### Task

- Use `**bold**` to highlight one keyword
- Use `>` to write a reminder you like
- Add a link to a webpage you want to visit
- Use a table to create a morning and afternoon schedule
- Use a horizontal rule to separate the schedule from the reminder

---

## 12 - Mathematical Notation: Inline and Display Math

<style scoped>
section {
  font-size: 18px;
}
section h3 {
  margin: 10px 0 4px;
  font-size: 20px;
}
section p {
  margin: 0.35em 0;
}
section pre {
  margin: 7px 0 9px;
  padding: 40px 18px 10px;
  font-size: 17px;
  line-height: 1.3;
}
section pre::before {
  height: 30px;
}
</style>

Markdown commonly uses LaTeX-style syntax for mathematical notation. Whether the notation renders depends on the reading tool; in VS Code, check the result in the preview pane on the right.

### Inline math

Wrap a short expression in one pair of `$` symbols to keep it in the same line as a sentence:

```markdown
The mass-energy equation is $E = mc^2$, where $c$ is the speed of light.
```

### Display math

For a longer equation or one that needs emphasis, use two pairs of `$$` on separate lines:

```markdown
$$
x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}
$$
```

*Opening and closing delimiters must be paired. For display math, place each `$$` on its own line.*

---

## 13 - Mathematical Notation: Common Syntax

| Purpose | Markdown syntax | Rendered result |
| --- | --- | --- |
| Superscripts and subscripts | `$x^2$`, `$a_1$` | $x^2$, $a_1$ |
| Fractions | `$\frac{a}{b}$` | $\frac{a}{b}$ |
| Square and nth roots | `$\sqrt{x}$`, `$\sqrt[n]{x}$` | $\sqrt{x}$, $\sqrt[n]{x}$ |
| Summation | `$\sum_{i=1}^{n}x_i$` | $\sum_{i=1}^{n}x_i$ |
| Greek letters | `$\alpha$`, `$\beta$` | $\alpha$, $\beta$ |

Curly braces `{}` group several characters together. For example, `x^{10}` produces $x^{10}$, while `x^10` normally applies the superscript only to the character immediately following it.

A complete mean formula can be written as:

$$
\bar{x} = \frac{1}{n}\sum_{i=1}^{n}x_i
$$

---

<!-- _class: activities -->

## Exercise 04 - Write a Mathematical Expression

### Basics

- Write a sentence containing inline math: `The area of a circle is $S = \pi r^2$`
- Use display math to write the Pythagorean theorem: `a^2 + b^2 = c^2`

### Practice

- Write the mean of three numbers: `\frac{a+b+c}{3}`
- Write a square root: `\sqrt{9} = 3`

### Check

- Are `$` and `{}` correctly paired?
- Does the preview display a formula rather than the source code?

---

## 14 - Images: Insertion and Alt Text

<style scoped>
section {
  font-size: 19px;
}
section pre {
  margin: 10px 0;
  padding: 46px 22px 14px;
  font-size: 18px;
  line-height: 1.35;
}
section table {
  margin: 10px 0 6px;
  font-size: 18px;
}
section th,
section td {
  padding: 6px 12px;
}
</style>

Standard Markdown inserts an image with `![alt text](image path)`. Alt text appears when an image cannot load and helps readers understand what the image shows.

```markdown
![Ginkgo trees on campus](assets/ginkgo.jpg)
![Markdown logo](https://example.com/markdown.png)
```

| Part | Purpose | Example |
| --- | --- | --- |
| `!` | Indicates an image | Must come first |
| `[]` | Holds alt text describing the image | `Ginkgo trees on campus` |
| `()` | Holds the image path or URL | `assets/ginkgo.jpg` |

*If an image does not load, first check the file name, folder name, and path.*

---

## 15 - Images: Paths and Links

<style scoped>
section {
  font-size: 19px;
}
</style>

Local images are usually referenced with relative paths. Keeping them in a dedicated folder makes a Markdown project easier to organise and share.

```markdown
![Course cover](assets/cover.png)
![Flowchart](../images/flowchart.png)
[![Project home](assets/logo.png)](https://example.com)
```

- `photo.png`: the image and Markdown file are in the same folder
- `assets/photo.png`: the image is in the current folder's `assets` subfolder
- `../images/photo.png`: move up one folder, then into `images`
- `[![...](...)](URL)`: makes an image clickable and links to a webpage

> **Tip:** Use brief, accurate alt text and keep course images together in an `assets` folder.

---

<!-- _class: activities -->

## Exercise 05 - Insert and Describe an Image

### Task

- Put an image into the `assets` folder
- Insert it with `![a short description](assets/your-image-file.png)`
- Write alt text that clearly describes the image
- Optional: wrap the image in a link that opens a related webpage

### Check

- Does it start with `!`, and are `[]` and `()` correctly paired?
- Is the image path inside the parentheses `(...)`?
- Would the alt text help someone who cannot see the image?

---

<!-- _class: yellow -->

## PART 04

### 04

#### Practice & Review

Put the techniques you have learned into one note, then revisit the core ideas

---

<!-- _class: activities -->

## 16 - Write a Personal Introduction Card

### Task

- Use `##` to write `About Me`
- Use an unordered list for your major, interests, and a recent goal
- Highlight one item with `**bold**`
- Add a link to a website you visit often

### Self-check

- Is there a space after every `#`, `-`, and `1.`?
- Does every link follow the format `[label](URL)`?
- Does each line express only one piece of information?

---

## 17 - Clear Writing Beats Complicated Writing

```markdown
## About Me

- **Major**: Computer Science
- Interest: Programming
- Recent goal: [Learn Markdown](https://www.markdownguide.org/)
```

- A heading should name the topic; it does not need to be a complete sentence
- Try to express only one idea per line
- Use meaningful link text instead of pasting bare URLs
- Formatting should make reading easier, not show how many symbols you remember

---

<!-- _class: todo -->

## 18 - Summary and Review

### Core Syntax

- Headings, paragraphs, and ordered or unordered lists give content structure
- Bold, italics, links, and inline code highlight important information
- Quotations, tables, and horizontal rules organise different kinds of content
- Use `$...$` or `$$...$$` for math, and `![alt text](image path)` for images

### Writing Principles

- Decide on the content structure before choosing Markdown syntax
- Keep the source clear and readable; use preview when you need to check the result
- Use brief, accurate wording so readers can find the key points easily

Markdown is about clear structure, not memorising syntax.

---

<!-- _class: yellow -->

## THANK YOU

### Q&A

#### Let's Write Markdown

Computer Psycho Union - A Quick Introduction to Markdown
