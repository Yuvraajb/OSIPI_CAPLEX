# OSIPI CAPLEX Quick Reference

This quick reference provides common syntax and patterns used in OSIPI CAPLEX Markdown files.

## Basic Markdown

| Element | Syntax |
| ------- | ------ |
| Heading 1 | `# Heading` |
| Heading 2 | `## Heading` |
| Heading 3 | `### Heading` |
| Bold | `**bold text**` |
| Italic | `*italic text*` |
| Link | `[link text](URL)` |
| Image | `![alt text](image.jpg)` |
| Blockquote | `> quoted text` |
| Ordered List | `1. First item` <br> `2. Second item` |
| Unordered List | `- Item` <br> `- Another item` |
| Code | `` `code` `` |
| Code Block | ``````` <br> ```language <br> code <br> ``` <br> ``````` |
| Horizontal Rule | `---` |

## CAPLEX-Specific Elements

### Anchors and Links

Create an anchor:
```
<a id="uniqueID"></a>
```

Link to an anchor:
```
[link text](#uniqueID)
```

Link to an anchor on another page:
```
[link text](page.md#uniqueID){target="_blank"}
```

### Tables

Basic table structure:
```
| Header 1 | Header 2 | Header 3 |
| -------- | -------- | -------- |
| Cell 1   | Cell 2   | Cell 3   |
```

Multi-line cell content:
```
| Header 1 | Header 2 |
| -------- | -------- |
| Cell 1   | Line 1<br>Line 2 |
```

### Hyperlink Button

```
<button class="md-button md-button--hyperlink">COPY LINK</button>
```

### Math Equations

Inline math:
```
$equation$
```

Display math:
```
$$
equation
$$
```

### Material MkDocs Extensions

Note box:
```
!!! note "Optional Title"
    Note content
```

Warning box:
```
!!! warning
    Warning content
```

Expandable section:
```
??? question "Title"
    Hidden content
```

Tabbed content:
```
=== "Tab 1"
    Tab 1 content

=== "Tab 2"
    Tab 2 content
```

Annotations:
```
Text to annotate (1)
{ .annotate }

1. Annotation content
```

### Common Lexicon Patterns

Quantity entry:
```
| Q.XX1.001 <button class="md-button md-button--hyperlink">COPY LINK</button> | <a id="ID"></a> Name | Alt Names | *Symbol* | Description | Units | Reference |
```

Model entry:
```
| M.XX1.001 <button class="md-button md-button--hyperlink">COPY LINK</button> | <a id="ID"></a> Name | Alt Names | Symbol | Description | Reference |
```

### Images with Options

```
![alt text](image.jpg){ width="300" }
![alt text](image.jpg){ align=right }
![alt text](image.jpg){ loading=lazy }
```

## Common Quantities Notation

| Quantity | Notation |
| -------- | -------- |
| Signal | *S* |
| T1 | *T<sub>1</sub>* |
| T2 | *T<sub>2</sub>* |
| T2* | *T<sub>2</sub><sup>*</sup>* |
| R1 | *R<sub>1</sub>* |
| R2 | *R<sub>2</sub>* |
| R2* | *R<sub>2</sub><sup>*</sup>* |

## HTML Elements for Layout

Two-column layout:
```html
<div class="grid" markdown>
<div class="grid-column" markdown>

First column content (written in Markdown)

</div>
<div class="grid-column" markdown>

Second column content (written in Markdown)

</div>
</div>
```

Centered image:
```html
<div class="center-image" markdown>
![alt text](image.jpg)
</div>
```
