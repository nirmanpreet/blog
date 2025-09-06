---
title: "Ultimate Hugo + Hextra Formatting Showcase"
date: 2025-09-06
authors:
  - name: "Nirmanpreet Singh"
tags: ["hugo", "hextra", "markdown", "showcase"]
toc: true
summary: "This test article demonstrates all formatting, shortcodes, and features supported by Hugo + Hextra."
slug: "ultimate-showcase"
---

<!--more-->

# Hugo + Hextra Formatting Showcase 🎉

Welcome to the **ultimate test post**.  
This file demonstrates everything from **Markdown basics** to **Hugo templating magic**.

---

## 1. Headings & Text Styles

# H1 Heading
## H2 Heading
### H3 Heading with *italic*
#### H4 Heading with **bold**

Text styles: *italic*, **bold**, ***bold italic***, ~~strikethrough~~  

Subscript: H<sub>2</sub>O  
Superscript: E = mc<sup>2</sup>

---

## 2. Quotes & Alerts

> Normal blockquote  
>> Nested blockquote

> [!NOTE] This is a note  

> [!TIP] This is a tip

> [!IMPORTANT] Important info  

> [!WARNING] Warning message  

> [!CAUTION] Be careful!

---

## 3. Lists

### Ordered
1. First
2. Second
   1. Nested
   2. Nested
3. Third

### Unordered
- Item
- Another item
  - Sub-item

### Tasks
- [ ] Not done
- [x] Done

---

## 4. Tables

| Name   | Age | Status      |
| :----- | --: | :---------- |
| Alice  |  23 | *Student*   |
| Bob    |  27 | **Engineer**|
| Carol  |  30 | ~~Retired~~ |

---

## 5. Links & Cross References

- External: [Markdown Guide](https://www.markdownguide.org)  
- Internal: [Jump to Shortcodes](#10-shortcodes)  

---

## 6. Images

### Markdown Image
![Nature](https://source.unsplash.com/400x300/?nature "Nature")

### Hugo Figure
{{< figure src="https://source.unsplash.com/600x400/?mountain" caption="Hugo Figure with Caption" width="400" >}}

---

## 7. Code Examples

### Inline
Here’s some `inline code`.

### Code Block
```python {filename="hello.py" linenos=table hl_lines=[2]}
def say_hello():
    print("Hello World")
```

### Hugo Highlight
{{< highlight html >}}
<p>Hello with Hugo highlight</p>
{{< /highlight >}}

---

## 8. Footnotes

This text has a footnote.[^1]

[^1]: This is the footnote.

---

## 9. Summaries & Read More

Content above `<!--more-->` is used as **summary** in lists.  
Below is extra content for detail pages.

---

## 10. Shortcodes

### Callouts
{{< callout type="info" >}}
This is an **Info Callout**.
{{< /callout >}}

### Cards
{{< cards cols="2" >}}
{{< card title="Card 1" link="/" icon="github" subtitle="Basic Card" >}}
{{< card title="Card 2" subtitle="With Image" image="https://source.unsplash.com/400x250/?tech" >}}
{{< /cards >}}

### Collapsible Details
{{< details "Click to reveal hidden text" >}}
This text is **hidden by default**.
{{< /details >}}

### Mermaid Diagram
```mermaid
graph TD;
  A[Start] --> B{Choice?};
  B -->|Yes| C[Path 1];
  B -->|No| D[Path 2];
```

### File Tree
{{< filetree/container >}}
  {{< filetree/folder name="content" >}}
    {{< filetree/file name="_index.md" >}}
  {{< /filetree/folder >}}
  {{< filetree/file name="hugo.toml" >}}
{{< /filetree/container >}}

### Icons
GitHub icon: {{< icon "github" >}}



Block math:
$$
F(\omega) = \int_{-\infty}^\infty f(t)e^{-j\omega t}dt
$$

### Badges
{{< badge "New" >}}  
{{< badge content="Releases" link="https://github.com/imfing/hextra/releases" icon="github" >}}

### YouTube
{{< youtube dQw4w9WgXcQ >}}

### PDF Embed
{{< pdf "https://www.w3.org/WAI/ER/tests/xhtml/testfiles/resources/pdf/dummy.pdf" >}}

### Steps
{{% steps %}}

### Step 1
Install Hugo
### Step 2
Create a new site
### Step 3
Run `hugo server`
{{% /steps %}}

### Tabs
{{< tabs items="YAML,JSON" defaultIndex="0" >}}
{{< tab >}}
```yaml
title: "My Site"
theme: "hextra"
```
{{< /tab >}}
{{< tab >}}
```json
{
  "title": "My Site",
  "theme": "hextra"
}
```
{{< /tab >}}
{{< /tabs >}}

---

# ✅ Done

This demo shows:  
- **Markdown basics**  
- **Hugo formatting & features**  
- **Hextra shortcodes**  

Use this as your **template** for future articles.
