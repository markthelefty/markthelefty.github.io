---
title: Pattern Library
date: 2018-07-30 14:00:00 -04:00
description: Every publication, application and organization can benefit from having
  consistent branding and design patterns. It takes some time and effort to build
  a complete pattern library, but the effort is worth it. This is the Mark On Product
  pattern library - hopefully it's useful.
image: v1533634577/social-images/pattern-library-social-image.jpg
readtime: 9
---

The purpose of this pattern library is to serve as a reference for how commonly used components should be marked up and styled. Mark On Product is written using [Markdown](https://daringfireball.net/projects/markdown/). Most core components are written using [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/). Many of the common patterns are detailed below, this [cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) is also helpful. The [GitHub Markdown](https://help.github.com/categories/writing-on-github/) documentation also serves as a great reference.

Mark On Product is built using [Jekyll](https://jekyllrb.com/), the theme is built from [Lanyon](http://lanyon.getpoole.com/) and has been heavily customized.
<br>

## Colors
{: .divider}
There are several core "brand" colors, two primary colors and one secondary color.

![Style Guide Brand Colors](https://res.cloudinary.com/dbrkuvff5/image/upload/f_auto,q_auto/v1533289307/post-images/colors.png)

```css
.brand-green {color: #67a43e}
.brand-black {color: #272727}
.background-white {color: #fafafa}
```  
<br/>

## Typography
{: .divider}
The fonts choices are intentionally limited and each has a specific purpose. Post Titles `h1` are set in Myriad Pro. Post Subpage Titles `h2`, Section Headers `h3`, and Subsection Headers `h4` are all set in PT Sans.

### Headings
# Post Titles (h1)
{: .post-title}
```markdown
# Post Title (h1)
font-family: Myriad Pro
```
## Subpage Title (h2)
```markdown
## Subpage Title (h2)
font-family: Source Sans Pro
```
### Section Header (h3)
```markdown
### Section Header (h3)
font-family: Source Sans Pro
```
#### Subsection Header (h4)
```markdown
#### Subsection Header (h4)
font-family: Source Sans Pro
```
<br/>
### Paragraph
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin aliquet sed magna et sodales. Vestibulum vehicula dolor sit amet luctus viverra. Praesent facilisis dictum sapien, et elementum lorem imperdiet pulvinar. Nulla lacinia, arcu eget venenatis dapibus, neque tellus vestibulum elit, tempor condimentum turpis elit a justo.
```css
{font-family: "source-sans-pro";
color: #1f1f1f;
font-size: 20px;
font-weight: 300;
line-height: 32px;}
```

### Paragraph Lead Text
<span class="lead">Lorem ipsum dolor sit amet, consectetur adipiscing elit.</span> Proin aliquet sed magna et sodales. Vestibulum vehicula dolor sit amet luctus viverra. Praesent facilisis dictum sapien, et elementum lorem imperdiet pulvinar.
```html
<span class="lead">Lead Text</span>
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
Abbreviations, like <abbr title="absent without leave">AWOL</abbr> should use `<abbr>`, with an optional `title` attribute for the full phrase.
```html
<abbr title="absent without leave">AWOL</abbr>
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

### Superscript Text
Superscript <sup>text</sup> uses `<sup>`.
```html
Superscript <sup>text</sup>
```

### Subscript Text
Subscript <sub>text</sub> uses `<sub>`.
```html
Subscript <sub>text</sub>
```
<br/>

## Code Stlyes
{: .divider}
Code markup is automatically applied by the Markdown parser as long as the correct code type is added. Styles are handled by [Pygments](http://jwarby.github.io/jekyll-pygments-themes/languages/javascript.html) via the `syntax.css` stylesheet.

### Inline
Inline `code` has (*back-ticks*) around it.
```markdown
`code`
```

### Markdown
```markdown
### H3 Example
```

### CSS
```css
.brand-green {color: #67a43e}
```

### HTML
```html
<h2 class="brand-green">Post Subtitle</h2>
```
<br/>

## Lists
{: .divider}
There are four lists styles supported. Unordered lists, ordered lists, mixed lists, and definition lists. All lists can be written in Markdown except for definition lists, they are written in HTML.

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

### Mixed Lists
1. Praesent commodo cursus magna, vel scelerisque consectetur et.
   * Mixed Item One
   * Mixed Item Two
2. Donec id elit non mi porta gravida at eget metus.

```markdown
1. Praesent commodo cursus magna, vel scelerisque consectetur et.
   * Mixed Item One
   * Mixed Item Two
2. Donec id elit non mi porta gravida at eget metus.
```

### Definition Lists
<dl>
  <dt>Aluminum</dt>
  <dd>Aluminium or aluminum is a chemical element with symbol Al and atomic number 13. It is a silvery-white, soft, nonmagnetic and ductile metal in the boron group.</dd>

  <dt>Brass</dt>
  <dd>Brass is a metallic alloy that is made of copper and zinc. The proportions of zinc and copper can vary to create different types of brass alloys with varying mechanical and electrical properties.</dd>

  <dt>Copper</dt>
  <dd>Copper is a chemical element with symbol Cu (from Latin: cuprum) and atomic number 29. It is a soft, malleable, and ductile metal with very high thermal and electrical conductivity.</dd>
</dl>
```html
<dl>
  <dt>Aluminum</dt>
  <dd>Aluminium or aluminum is a chemical element with symbol Al and atomic number 13. It is a silvery-white, soft, nonmagnetic and ductile metal in the boron group.</dd>

  <dt>Brass</dt>
  <dd>Brass is a metallic alloy that is made of copper and zinc. The proportions of zinc and copper can vary to create different types of brass alloys with varying mechanical and electrical properties.</dd>

  <dt>Copper</dt>
  <dd>Copper is a chemical element with symbol Cu (from Latin: cuprum) and atomic number 29. It is a soft, malleable, and ductile metal with very high thermal and electrical conductivity.</dd>
</dl>
```
<br/>

## Tables
{: .divider}
Tables used are fairly simple, nothing too tricky. 

### Standard Left Aligned

| Company | Contact | Country |
| --- | --- | --- |
| Alfreds Futterkiste | Maria Anders | Germany |
| Centro Moctezuma | Francisco Chang | Mexico |
| Ernst Handel | Roland Mendel | Austria |
| Island Trading | Helen Bennett | UK |

```markdown
| Company | Contact | Country |
| --- | --- | --- |
| Alfreds Futterkiste | Maria Anders | Germany |
| Centro Moctezuma | Francisco Chang | Mexico |
| Ernst Handel | Roland Mendel | Austria |
| Island Trading | Helen Bennett | UK |
```

### Mixed Alignment

| Company | Contact | Country |
| --- | :---: | ---: |
| Left Aligned | Center Aligned | Right Aligned |
| Centro Moctezuma | Francisco Chang | Mexico |
| Ernst Handel | Roland Mendel | Austria |
| Island Trading | Helen Bennett | UK |

```markdown
| Company | Contact | Country |
| --- | :---: | ---: |
| Left Aligned | Center Aligned | Right Aligned |
| Centro Moctezuma | Francisco Chang | Mexico |
| Ernst Handel | Roland Mendel | Austria |
| Island Trading | Helen Bennett | UK |
```
<br/>

## Links
{: .divider}
Links will [look like this](http://example.com), nice and simple.
```markdown
[Linked Text](http://url.com)
```
<br/>

## Image Sizing and Formatting
{: .divider}
Images can be sized using [this Sketch template](https://res.cloudinary.com/dbrkuvff5/raw/upload/v1533594760/post-files/post-image-template.sketch). There's no secret to the sizing, but using this template will ensure consistency across posts and social media cards.

The width is set by adding a class that divides the total column width by 8. `.width-1`, `.width-2`, `.width-3`, `.width-4`, `.width-5`, `.width-6`, `.width-7`, `.width-8`. Images are 100% wide by default so adding a width class isn't necessary. On small (*mobile sized*) screens all images are 100% wide by default.

All image filetypes are acceptable, but care should be taken to ensure the appropriate types are being used. `.jpg` should be used for photos and `.png` should be used for design assets (*like logos*). 

Cloudinary will serve the smallest filetype and size automatically as long as the `.cld-responsive` class is added.

### 12.5% Width
![Image 12.5% Wide](https://res.cloudinary.com/dbrkuvff5/image/upload/f_auto,q_auto/c_scale,q_auto:good,w_845/v1534292126/post-images/sample-post-image.jpg){: .width-1}
```markdown
![Alt Text](img/url){: .width-1}
```

### 25% Width
![Image 25% Wide](https://res.cloudinary.com/dbrkuvff5/image/upload/f_auto,q_auto/c_scale,q_auto:good,w_845/v1534292126/post-images/sample-post-image.jpg){: .width-2}
```markdown
![Alt Text](img/url){: .width-2}
```

### 37.5% Width
![Image 37.5% Wide](https://res.cloudinary.com/dbrkuvff5/image/upload/f_auto,q_auto/c_scale,q_auto:good,w_845/v1534292126/post-images/sample-post-image.jpg){: .width-3}
```markdown
![Alt Text](img/url){: .width-3}
```

### 50% Width
![Image 50% Wide](https://res.cloudinary.com/dbrkuvff5/image/upload/f_auto,q_auto/c_scale,q_auto:good,w_845/v1534292126/post-images/sample-post-image.jpg){: .width-4}
```markdown
![Alt Text](img/url){: .width-4}
```

### 62.5% Width
![Image 62.5% Wide](https://res.cloudinary.com/dbrkuvff5/image/upload/f_auto,q_auto/c_scale,q_auto:good,w_845/v1534292126/post-images/sample-post-image.jpg){: .width-5}
```markdown
![Alt Text](img/url){: .width-5}
```

### 75% Width
![Image 75% Wide](https://res.cloudinary.com/dbrkuvff5/image/upload/f_auto,q_auto/c_scale,q_auto:good,w_845/v1534292126/post-images/sample-post-image.jpg){: .width-6}
```markdown
![Alt Text](img/url){: .width-6}
```

### 87.5% Width
![Image 87.5% Wide](https://res.cloudinary.com/dbrkuvff5/image/upload/f_auto,q_auto/c_scale,q_auto:good,w_845/v1534292126/post-images/sample-post-image.jpg){: .width-7}
```markdown
![Alt Text](img/url){: .width-7}
```

### 100% Width
![Image 100% Wide](https://res.cloudinary.com/dbrkuvff5/image/upload/f_auto,q_auto/c_scale,q_auto:good,w_845/v1534292126/post-images/sample-post-image.jpg){: .width-8}
```markdown
![Alt Text](img/url){: .width-8}
```

### 25% Width (Float Left)
![Image 25% Wide](https://res.cloudinary.com/dbrkuvff5/image/upload/f_auto,q_auto/c_scale,q_auto:good,w_845/v1534292126/post-images/sample-post-image.jpg){: .width-2 .float-left}
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin aliquet sed magna et sodales. Vestibulum vehicula dolor sit amet luctus viverra. Praesent facilisis dictum sapien, et elementum lorem imperdiet pulvinar. Nulla lacinia, arcu eget venenatis dapibus, neque tellus vestibulum elit, tempor condimentum turpis elit a justo.
```markdown
![Alt Text](img/url){: .width-2 .float-left}
```

### 25% Width (Float Right)
![Image 25% Wide](https://res.cloudinary.com/dbrkuvff5/image/upload/f_auto,q_auto/c_scale,q_auto:good,w_845/v1534292126/post-images/sample-post-image.jpg){: .width-2 .float-right}
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin aliquet sed magna et sodales. Vestibulum vehicula dolor sit amet luctus viverra. Praesent facilisis dictum sapien, et elementum lorem imperdiet pulvinar. Nulla lacinia, arcu eget venenatis dapibus, neque tellus vestibulum elit, tempor condimentum turpis elit a justo.
```markdown
![Alt Text](img/url){: .width-2 .float-right}
```

### 50% Width (Float Left)
![Image 50% Wide](https://res.cloudinary.com/dbrkuvff5/image/upload/f_auto,q_auto/c_scale,q_auto:good,w_845/v1534292126/post-images/sample-post-image.jpg){: .width-4 .float-left}
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin aliquet sed magna et sodales. Vestibulum vehicula dolor sit amet luctus viverra. Praesent facilisis dictum sapien, et elementum lorem imperdiet pulvinar. Nulla lacinia, arcu eget venenatis dapibus, neque tellus vestibulum elit, tempor condimentum turpis elit a justo.
```markdown
![Alt Text](img/url){: .width-4 .float-left}
```

### 75% Width (Float Left)
![Image 75% Wide](https://res.cloudinary.com/dbrkuvff5/image/upload/f_auto,q_auto/c_scale,q_auto:good,w_845/v1534292126/post-images/sample-post-image.jpg){: .width-6 .float-left}
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin aliquet sed magna et sodales. Vestibulum vehicula dolor sit amet luctus viverra. Praesent facilisis dictum sapien, et elementum lorem imperdiet pulvinar. Nulla lacinia, arcu eget venenatis dapibus, neque tellus vestibulum elit, tempor condimentum turpis elit a justo.
```markdown
![Alt Text](img/url){: .width-6 .float-left}
```

### Linked Image
[![Linked Image](https://res.cloudinary.com/dbrkuvff5/image/upload/f_auto,q_auto/c_scale,q_auto:good,w_845/v1534292126/post-images/sample-post-image.jpg)](http://www.example.com/ "Example Title")
```markdown
[![Linked Image](https://res.cloudinary.com/dbrkuvff5/image/upload/f_auto,q_auto/c_scale,q_auto:good,w_845/v1534292126/post-images/sample-post-image.jpg)](http://www.example.com/ "Example Title")
```

### Cloudinary URLs
[Cloudinary](https://cloudinary.com/) is used for all image and asset hosting. Use the code below to automatically build the URLs and add the correct parameters for the image size and quality.
```markdown
![Alt Text](https://res.cloudinary.com/dbrkuvff5/image/upload/f_auto/c_scale,q_auto:good,w_845/[file_number]/[folder_name]/[file_name])
```
The `w_845` parameter determines the image width. It can be set to any width, in general it should be set to match the width class.

The `q_auto:good` parameter determines the image quality the available options are: `q_auto:best` , `:good`, `:eco`, or `:low`.
<br/>

## Horizontal Rules and Dividers
{: .divider}
In most cases dividing lines will be added by default as part of the design. In scenarios where you'd like to add a divider manually, there's two ways to do it.

The first is to add class `.divider`. This should be used to add a divider to an HTML element.

### h3 With a Divider
{: .divider}

### Image With a Divider
![Image 100% Wide](https://res.cloudinary.com/dbrkuvff5/image/upload/f_auto,q_auto/v1533119534/post-images/post-image-sample-100.png){: .cld-responsive .width-100 .divider}

```markdown
### h3 With a Divider
{: .divider}
```

In circumstances when there isn't an element to add the divider class to, simply generate a `<hr>` using Markdown.

---
```markdown
---
```
<br/>

## Message Styles
{: .divider}
Messages can be used to call special attention to important content. Messages should not be longer than one or two short sentences.

To create a message, add `.message` to a paragraph. This defines the default style. To create a secondary, success, alert, or danger message add that as a second class. This concept is loosely based on how [Bootstrap](https://getbootstrap.com/docs/4.0/components/alerts/) styles alerts.

### Default Message
This is a default message.
{: .message}
```markdown
{: .message}
```

### Secondary Message
This is a secondary message.
{: .message .message-secondary}
```markdown
{: .message .message-secondary}
```

### Success Message
This is a success message.
{: .message .message-success}
```markdown
{: .message .message-success}
```

### Alert Message
This is an alert message.
{: .message .message-alert}
```markdown
{: .message .message-alert}
```

### Danger Message
This is a danger message.
{: .message .message-danger}
```markdown
{: .message .message-danger}
```

### Blockquotes
> "This is quoted text"

```markdown
> "This is quoted text"
```