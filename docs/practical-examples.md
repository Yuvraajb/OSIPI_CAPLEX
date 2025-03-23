# Practical Contribution Examples

This guide provides step-by-step examples of common contribution scenarios to help you get started with OSIPI CAPLEX.

## Example 1: Adding a New Lexicon Entry

Let's walk through the process of adding a new quantity to the lexicon.

### Step 1: Locate the Appropriate File

Quantities are stored in `docs/quantities.md`. Open this file in your editor.

### Step 2: Find the Correct Section

Quantities are organized alphabetically by category. For example, if you're adding a new "Signal" quantity, find the "Signal" section in the file.

### Step 3: Add Your Entry

Copy an existing table row and modify it with your new information:

```markdown
| Q.MS1.002.[j] <button class="md-button md-button--hyperlink">COPY LINK</button> | <a id="Snorm"></a> Normalized Signal | -- | *S<sub>norm,j</sub>* | The MR signal in compartment *j* normalized to a reference value. | a.u. | -- |
```

### Step 4: Preview Your Changes

With `mkdocs serve` running, check your browser to see how your new entry looks.

### Step 5: Commit Your Change

Follow the Git workflow to commit and push your change:

```
git add docs/quantities.md
git commit -m "Add normalized signal quantity to lexicon"
git push
```

## Example 2: Adding a New Reference

References can enhance the value of lexicon entries. Here's how to add one:

### Step 1: Find the Entry Needing a Reference

Locate the lexicon entry that needs a reference.

### Step 2: Add the Reference

Update the reference column with a properly formatted link:

```markdown
| Q.MS1.001.[j] <button class="md-button md-button--hyperlink">COPY LINK</button> | <a id="S"></a> Signal | -- | *S<sub>j</sub>* | The MR signal (magnitude, phase or complex depending on context) in compartment *j*. | a.u. | [Bernstein et al. (2004)](https://doi.org/10.1016/B978-0-12-092861-3.X5000-6) |
```

For DOI references, use the format:
```
[Author et al. (Year)](https://doi.org/10.xxxx/xxxxx)
```

For PubMed references, use:
```
[Author et al. (Year)](https://www.ncbi.nlm.nih.gov/pmc/articles/PMCxxxxxxx/)
```

## Example 3: Creating a New Section Page

If you need to add a completely new section to the website:

### Step 1: Create the Markdown File

Create a new `.md` file in the `docs` directory:

```
touch docs/new-section.md
```

### Step 2: Add Basic Content Structure

Start with a header and introduction:

```markdown
# New Section Title

This section covers [brief description of what this section is about].

## Overview

[Provide a general overview of the topic]

## Key Concepts

[List and describe the most important concepts in this area]
```

### Step 3: Update Navigation

Add your new page to the `mkdocs.yml` file in the `nav:` section:

```yaml
nav:
  - Home: index.md
  - Quantities: quantities.md
  - Your New Section: new-section.md
```

## Example 4: Adding Interactive Elements

MkDocs Material offers various interactive elements to enhance your content:

### Adding Expandable Content

Use this pattern to create content that expands when clicked:

```markdown
??? example "Click to expand"
    This content is hidden by default.
    
    It can contain multiple paragraphs, code blocks, and even images.
    
    ```python
    def example():
        return "This is a code example"
    ```
```

### Adding Tabbed Content

Create tabbed sections like this:

```markdown
=== "Basic Usage"
    Here's the basic way to use this feature.
    
=== "Advanced Options"
    For more control, try these advanced settings.
    
=== "Examples"
    See these examples of the feature in action.
```

## Example 5: Styling and Formatting

Here are some examples of styling options:

### Text Formatting

```markdown
**Bold text** for emphasis
*Italic text* for slight emphasis
`code` for inline code references
```

### Block Elements

```markdown
> This is a blockquote.
> It can span multiple lines.

```python
# This is a code block with syntax highlighting
def function():
    return "Hello World"
```

!!! tip
    This is a tip callout box.
```

### Mathematical Equations

For inline equations:
```markdown
The relationship is defined by $E = mc^2$ where $m$ is mass.
```

For display equations:
```markdown
$$
R_1 = \frac{1}{T_1}
$$
```

## Getting Help

If you run into issues with any of these examples, please:

1. Refer to the [MkDocs Material documentation](https://squidfunk.github.io/mkdocs-material/reference/)
2. Ask for help in the [GitHub Issues section](https://github.com/OSIPI/OSIPI_CAPLEX/issues)
