---
title: Theme Style Guide
date: 2018-07-30 14:00:00 -04:00
description: This is a post META description. New!!
image: https://res.cloudinary.com/dbrkuvff5/image/upload/v1532890567/social-images/linkedin-post-img-test.jpg
---

Mark On Product is written using [Markdown](https://daringfireball.net/projects/markdown/). The content on the pages use a good amount of [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/). Most of the core components are detailed below, this [cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) is also helpful. The [GitHub Markdown](https://help.github.com/categories/writing-on-github/) documentation is also a great reference.

## Colors
{: .divider}
The goal is to use several core "brand" colors. Currently there are two primary colors and one secondary color.

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
<span class="lead">
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
<br/>

## Links
{: .divider}
Links will [look like this](http://example.com).
```markdown
[Linked Text](http://url.com)
```
<br/>

## Image Styles
{: .divider}

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

### Cloudinary Urls
[Cloudinary](https://cloudinary.com/) is used for all image and asset hosting. Use the code below to automatically build the URLs and add the correct classes.
```markdown
![Alt Text](https://res.cloudinary.com/dbrkuvff5/image/upload/f_auto,q_auto/[file_number]/[folder_name]/[file_name]){: .cld-responsive}
```
<br/>

## HTML Elements
{: .divider}
<br/>

## Dividers
Page content can be divided using the following two methods.

Add `.divider` class to an element:

### H3 Example
{: .divider}

### Image Example
![Image 100% Wide](https://res.cloudinary.com/dbrkuvff5/image/upload/f_auto,q_auto/v1533119534/post-images/post-image-sample-100.png){: .cld-responsive .width-100 .divider}

```markdown
{: .divider}
```

### Use `<hr>` HTML element.

<hr>
```html
<hr>
```
<br/>

## Message Styles
{: .divider}

### Message Style 1

### Blockquote

<a id='F0QtxjUKTjpmffnIiEfubQ' class='gie-single' href='http://www.gettyimages.com/detail/967257354' target='_blank' style='color:#a7a7a7;text-decoration:none;font-weight:normal !important;border:none;display:none;'>Embed From Getty Mark</a><script>window.gie=window.gie||function(c){(gie.q=gie.q||[]).push(c)};gie(function(){gie.widgets.load({id:'F0QtxjUKTjpmffnIiEfubQ',sig:'xKey1WiaocDutFw_24b8okF5XaDzurpu8oCQ_JCx93Q=',w:'594px',h:'414px',items:'967257354',caption: true ,tld:'com',is360: false })});</script><script src='//embed-cdn.gettyimages.com/widgets.js' charset='utf-8' async></script>