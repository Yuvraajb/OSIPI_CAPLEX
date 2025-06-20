# OSIPI CAPLEX Style Guide

This style guide provides guidelines to ensure consistency across all contributions to the OSIPI CAPLEX website.

## General Principles

- **Clarity**: Write content that is clear and accessible to both experts and newcomers
- **Precision**: Use technically accurate language and proper terminology
- **Consistency**: Follow established patterns for formatting and organization
- **Brevity**: Be concise while conveying necessary information

## Document Structure

### Page Headers

- Use title case for main headers (e.g., "Signal Modeling Approaches")
- Use sentence case for subheaders (e.g., "Common signal models")
- Structure documents with a clear hierarchy (H1 → H2 → H3)

### Sections

Organize content in a logical flow:
1. Introduction/Overview
2. Key Concepts
3. Detailed Information
4. Examples (where applicable)
5. References

## Lexicon Entries

### Quantities

Follow this format for quantity entries:

```
| Q.[Category].[Number].[j] | <a id="UniqueID"></a> Full Name | Alternative Names | Notation | Description | Units | Reference |
```

Where:
- `[Category]` is the two-letter category code
- `[Number]` is a sequential three-digit number
- `[j]` indicates if the quantity applies to a specific compartment
- `UniqueID` is a short, memorable identifier

### Models

Follow this format for model entries:

```
| M.[Category].[Number] | <a id="UniqueID"></a> Full Name | Alternative Names | Notation | Description | Reference |
```

### Descriptions

- Begin with a capital letter and end with a period
- Be concise but complete (ideally 1-2 sentences)
- Include key parameters and their meanings
- Use proper mathematical notation
- Link to related quantities when first mentioned

## Mathematical Notation

### Symbols

- Use consistent symbols across the lexicon
- Italicize variables (e.g., *S*, *T*, *R*)
- Use subscripts for specificity (e.g., *S<sub>0</sub>*)
- Use proper Greek letters where conventional (e.g., τ, θ)

### Equations

- Center standalone equations
- Number significant equations for reference
- Use consistent notation between text and equations
- Include units where appropriate

Example:
```
$$
S = S_0 \cdot e^{-TE/T_2^*}
$$
```

## References

### Format

Use consistent reference formatting:

- DOI references: `[Author et al. (Year)](https://doi.org/10.xxxx/xxxxx)`
- PubMed references: `[Author et al. (Year)](https://www.ncbi.nlm.nih.gov/pmc/articles/PMCxxxxxxx/)`
- Books: `[Author (Year). Title. Publisher.](URL if available)`

### Citation Style

- For one author: `Smith (2020)`
- For two authors: `Smith and Jones (2020)`
- For three or more authors: `Smith et al. (2020)`

## Language Guidelines

### Terminology

- Use established terminology from the field
- Provide alternative names where multiple terms exist
- Define abbreviations on first use
- Add common abbreviations to the abbreviations.md file

### Writing Style

- Use active voice where possible
- Avoid unnecessary jargon
- Define technical terms for newcomers
- Be consistent with spelling (use American English)
- Write in third person (avoid "you" and "we")

## Images and Figures

- Provide descriptive alt text for all images
- Use vector formats (SVG) when possible
- Include captions explaining key elements
- Maintain consistent styling across related figures
- Optimize image sizes for web viewing

## Examples and Code

- Include practical examples where helpful
- Use syntax highlighting for code blocks
- Comment code examples thoroughly
- Ensure code examples are functional

## Website-Specific Elements

### Interactive Elements

- Use expandable sections for supplementary information
- Use tabs for alternative approaches or implementations
- Include tooltips for technical terms

### Navigation

- Ensure logical placement in site hierarchy
- Use descriptive link text
- Avoid deep nesting of pages
- Consider the user's journey through the site

## Review Process

Before submitting contributions:

1. Check for technical accuracy
2. Verify that formatting is consistent with this style guide
3. Ensure all links work correctly
4. Preview the content in a local build
5. Review for grammar and spelling

## Accessibility

- Use sufficient color contrast
- Provide text alternatives for non-text content
- Create descriptive link text
- Use proper heading hierarchy
- Avoid relying solely on color to convey information
