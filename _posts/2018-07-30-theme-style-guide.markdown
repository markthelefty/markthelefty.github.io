---
title: Theme Style Guide
date: 2018-07-30 14:00:00 -04:00
description: This is a post META description. New!!
image: https://res.cloudinary.com/dbrkuvff5/image/upload/v1532890567/social-images/linkedin-post-img-test.jpg
---

## Colors
{: .divider}
The goal is to use several core "brand" colors. Currently there are two primary colors and one secondary color.
<img src="https://res.cloudinary.com/dbrkuvff5/image/upload/f_auto,q_auto/v1532952269/post-images/colors.png" alt="Style Guide Brand Colors" class="cld-responsive">
```css
.brand-green {color: #67a43e}
.brand-black {color: #272727}
.background-white {color: #fafafa}
```  
<br/>
## Typography
{: .divider}
The fonts choices are intentionally limited and each has a specific purpose.

### Headings
# Post Title (h1)
{: .post-title}
```markdown
# Post Title (h1)
font-family: Myriad Pro
```
## Post Subtitle (h2)
```markdown
## Post Subtitle (h2)
font-family: PT Sans
```
### Post Subtitle (h3)
```markdown
### Post Subtitle (h3)
font-family: PT Sans
```
#### Post Subtitle (h4)
```markdown
#### Post Subtitle (h4)
font-family: PT Sans
```
<br/>
### Paragraphs
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin aliquet sed magna et sodales. Vestibulum vehicula dolor sit amet luctus viverra. Praesent facilisis dictum sapien, et elementum lorem imperdiet pulvinar. Nulla lacinia, arcu eget venenatis dapibus, neque tellus vestibulum elit, tempor condimentum turpis elit a justo.
```css
{font-family: "source-sans-pro";
color: #393939;
font-size: 22px;
font-weight: 300;
line-height: 35.2px;}
```
### Italics
*Italics* can be used for emphasis.
```markdown
*Italics*
```
### Bold
**Bold text** can be used for stronger emphasis.
```markdown
**Bold text**
```

### Abbreviations
Abbreviations, like <abbr title="HyperText Markup Langage">HTML</abbr> should use `<abbr>`, with an optional `title` attribute for the full phrase.
```html
<abbr title="HyperText Markup Langage">HTML</abbr>
```

### Citations
Citations, like <cite>&mdash; Mark Mitchell</cite>, should use `<cite>`.
```html
<cite>&mdash; Mark Mitchell</cite>
```

### Deleted Text
<del>Deleted</del> text should use `<del>`.
```html
<del>Deleted</del>
```

### Inserted Text
<ins>Inserted</ins> text should use `<ins>`.
```html
<ins>Inserted</ins>
```

### Superscript <sup>text</sup>
Superscript <sup>text</sup> uses `<sup>`.
```html
Superscript <sup>text</sup>
```

### Subscript <sub>text</sub>
Subscript <sub>text</sub> uses `<sub>`.
```html
Subscript <sub>text</sub>
```
<br/>

## Code Stlyes
{: .divider}
Code styles are automatically applied by the Markdown parser as long as the correct code type is added.


### Code (Inline)
Inline `code` has `back-ticks around` it.
```markdown
`code`
```

### Code (Markdown)
```markdown
### H3 Example
```

### Code (CSS)
```css
.brand-green {color: #67a43e}
```

### Code (HTML)
```html
<h2 class="brand-green">Post Subtitle</h2>
```
<br/>

## Lists
{: .divider}

### Unordered Lists
* Praesent commodo cursus magna, vel scelerisque consectetur et.
* Donec id elit non mi porta gravida at eget metus.
* Nulla vitae elit libero, a pharetra augue.

```markdown
* Praesent commodo cursus magna, vel scelerisque consectetur et.
* Donec id elit non mi porta gravida at eget metus.
* Nulla vitae elit libero, a pharetra augue.
```

### Ordered Lists
1. Praesent commodo cursus magna, vel scelerisque consectetur et.
2. Donec id elit non mi porta gravida at eget metus.
3. Nulla vitae elit libero, a pharetra augue.

```markdown
1. Praesent commodo cursus magna, vel scelerisque consectetur et.
2. Donec id elit non mi porta gravida at eget metus.
3. Nulla vitae elit libero, a pharetra augue.
```

<br/>

## Tables
{: .divider}

| Company | Contact | Country |
| ------------- | ------------- | ------------- |
| Alfreds Futterkiste    | Maria Anders    | Germany    |
| Table cell    | Table cell    | Table cell    |
| Table cell    | Table cell    | Table cell    |
| Table cell    | Table cell    | Table cell    |

<br/>

## Links
{: .divider}

## Image Styles
{: .divider}

### Cloudinary Urls

<br/>

## Code Elements
{: .divider}

<br/>

## HTML Elements
{: .divider}

<br/>

## Message Styles
{: .divider}

### Message Style 1

### Blockquote


