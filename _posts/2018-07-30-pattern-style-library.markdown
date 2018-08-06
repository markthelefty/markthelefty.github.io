---
title: Pattern and Style Library
date: 2018-07-30 14:00:00 -04:00
description: This is a post META description. New!!
image: https://res.cloudinary.com/dbrkuvff5/image/upload/v1532890567/social-images/linkedin-post-img-test.jpg
---

The purpose of this library is to serve as a reference for how the commonly used components should be coded and styled. Mark On Product is written using [Markdown](https://daringfireball.net/projects/markdown/). The content is primarily written using [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/). Many of the core components are detailed below, this [cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) is also helpful. The [GitHub Markdown](https://help.github.com/categories/writing-on-github/) documentation is also a great reference.

Mark On Product is built using [Jekyll](https://jekyllrb.com/), the theme is built from [Lanyon](http://lanyon.getpoole.com/).
<br>

## Colors
{: .divider}
There are several core "brand" colors, currently there are two primary colors and one secondary color.

![Style Guide Brand Colors](https://res.cloudinary.com/dbrkuvff5/image/upload/f_auto,q_auto/v1533289307/post-images/colors.png){: .cld-responsive}

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
## Subpage Title (h2)
```markdown
## Subpage Title (h2)
font-family: PT Sans
```
### Section Header (h3)
```markdown
### Section Header (h3)
font-family: PT Sans
```
#### Sub Section Heading (h4)
```markdown
#### Sub Section Heading (h4)
font-family: PT Sans
```
<br/>
### Paragraph
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin aliquet sed magna et sodales. Vestibulum vehicula dolor sit amet luctus viverra. Praesent facilisis dictum sapien, et elementum lorem imperdiet pulvinar. Nulla lacinia, arcu eget venenatis dapibus, neque tellus vestibulum elit, tempor condimentum turpis elit a justo.
```css
{font-family: "source-sans-pro";
color: #393939;
font-size: 22px;
font-weight: 300;
line-height: 35.2px;}
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
Code styles are automatically applied by the parser as long as the correct code type is added.

### Inline
Inline `code` has `back-ticks around` it.
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
There are four lists styles supported. Unordered lists, ordered lists, mixed lists, and definition lists. All lists can be written in Markdown except for definition lists, they will require HTML.

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
The tables used are fairly simple, nothing too tricky. 

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
Images should be sized using [this Sketch template](https://res.cloudinary.com/dbrkuvff5/raw/upload/v1533548442/post-files/post-image-template.sketch). There's no secret to the sizing, but it will ensure consistency. There's four sizes, you should consider the final display size as a percentage of the full-body width i.e., 25% of the content container. 

The width is set by adding a class `.width-25`, `.width-50`, `.width-75` or `.width-100`. Images are 100% wide by default so adding it isn't necessary. All images are 100% wide (and can't be floated) on mobile device sized screens.

All image filetypes are acceptable, but care should be taken to ensure the appropriate types are being used. `.jpg` should be used for photos and `.png` should be used for design assets like logos. 

Cloudinary will serve the smallest file type and size automatically as long as the `.cld-responsive` class is added.

### 25% Width
![Image 25% Wide](https://res.cloudinary.com/dbrkuvff5/image/upload/f_auto,q_auto/v1533119534/post-images/post-image-sample-25.png){: .cld-responsive .width-25}
```markdown
![Alt Text](img/url){: .cld-responsive .width-25}
```

### 50% Width
![Image 50% Wide](https://res.cloudinary.com/dbrkuvff5/image/upload/f_auto,q_auto/v1533119534/post-images/post-image-sample-50.png){: .cld-responsive .width-50}
```markdown
![Alt Text](img/url){: .cld-responsive .width-50}
```

### 75% Width
![Image 75% Wide](https://res.cloudinary.com/dbrkuvff5/image/upload/f_auto,q_auto/v1533119534/post-images/post-image-sample-75.png){: .cld-responsive .width-75}
```markdown
![Alt Text](img/url){: .cld-responsive .width-75}
```

### 100% Width
![Image 100% Wide](https://res.cloudinary.com/dbrkuvff5/image/upload/f_auto,q_auto/v1533119534/post-images/post-image-sample-100.png){: .cld-responsive .width-100}
```markdown
![Alt Text](img/url){: .cld-responsive .width-100}
Note: 100% width is default so adding this class won't be needed in most cases.
```

### 25% Width (Float Left)
![Image 25% Wide](https://res.cloudinary.com/dbrkuvff5/image/upload/f_auto,q_auto/v1533119534/post-images/post-image-sample-25.png){: .cld-responsive .width-25 .float-left}
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin aliquet sed magna et sodales. Vestibulum vehicula dolor sit amet luctus viverra. Praesent facilisis dictum sapien, et elementum lorem imperdiet pulvinar. Nulla lacinia, arcu eget venenatis dapibus, neque tellus vestibulum elit, tempor condimentum turpis elit a justo.
```markdown
![Alt Text](img/url){: .cld-responsive .width-25 .float-left}
```

### 25% Width (Float Right)
![Image 25% Wide](https://res.cloudinary.com/dbrkuvff5/image/upload/f_auto,q_auto/v1533119534/post-images/post-image-sample-25.png){: .cld-responsive .width-25 .float-right}
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin aliquet sed magna et sodales. Vestibulum vehicula dolor sit amet luctus viverra. Praesent facilisis dictum sapien, et elementum lorem imperdiet pulvinar. Nulla lacinia, arcu eget venenatis dapibus, neque tellus vestibulum elit, tempor condimentum turpis elit a justo.
```markdown
![Alt Text](img/url){: .cld-responsive .width-25 .float-right}
```

### 50% Width (Float Left)
![Image 50% Wide](https://res.cloudinary.com/dbrkuvff5/image/upload/f_auto,q_auto/v1533119534/post-images/post-image-sample-50.png){: .cld-responsive .width-50 .float-left}
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin aliquet sed magna et sodales. Vestibulum vehicula dolor sit amet luctus viverra. Praesent facilisis dictum sapien, et elementum lorem imperdiet pulvinar. Nulla lacinia, arcu eget venenatis dapibus, neque tellus vestibulum elit, tempor condimentum turpis elit a justo.
```markdown
![Alt Text](img/url){: .cld-responsive .width-50 .float-left}
```

### 75% Width (Float Left)
![Image 75% Wide](https://res.cloudinary.com/dbrkuvff5/image/upload/f_auto,q_auto/v1533119534/post-images/post-image-sample-75.png){: .cld-responsive .width-75 .float-left}
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin aliquet sed magna et sodales. Vestibulum vehicula dolor sit amet luctus viverra. Praesent facilisis dictum sapien, et elementum lorem imperdiet pulvinar. Nulla lacinia, arcu eget venenatis dapibus, neque tellus vestibulum elit, tempor condimentum turpis elit a justo.
```markdown
![Alt Text](img/url){: .cld-responsive .width-75 .float-left}
```

### Linked Image
[![Linked Image](https://res.cloudinary.com/dbrkuvff5/image/upload/f_auto,q_auto/v1533119534/post-images/post-image-sample-100.png){: .cld-responsive}](http://www.example.com/ "Example Title")
```markdown
[![Linked Image](https://res.cloudinary.com/dbrkuvff5/image/upload/f_auto,q_auto/v1533119534/post-images/post-image-sample-100.png){: .cld-responsive}](http://www.example.com/ "Example Title")
```

### Cloudinary Urls
[Cloudinary](https://cloudinary.com/) is used for all image and asset hosting. Use the code below to automatically build the URLs and add the `.cld-responsive` class.
```markdown
![Alt Text](https://res.cloudinary.com/dbrkuvff5/image/upload/f_auto,q_auto/[file_number]/[folder_name]/[file_name]){: .cld-responsive}
```
<br/>

## Dividers
{: .divider}
In most cases dividing lines will be added by default as part of the design. In scenarios where you'd like to add a divider manually there's two ways to ways to do it.

The first is to add `.divider` class to an element. This should be used to add a divider to an HTML element.

### H3 Example
{: .divider}

### Image Example
![Image 100% Wide](https://res.cloudinary.com/dbrkuvff5/image/upload/f_auto,q_auto/v1533119534/post-images/post-image-sample-100.png){: .cld-responsive .width-100 .divider}

```markdown
### H3 Example
{: .divider}
```

In circumstances when there isn't an element to add the divider class to, simply generate a `<hr>`.

---
```markdown
---
```
<br/>

## Message Styles
{: .divider}
Messages can be used to highlight certain items or call special attention to particular content. Messages should not be longer than one or two short sentences.

To create a message, add `.message` to a paragraph. This defines the default style. To create a secondary, success, alert, or danger message add that as a second class.

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
This is a secondary message.
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