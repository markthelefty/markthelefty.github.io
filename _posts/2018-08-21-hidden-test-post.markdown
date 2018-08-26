---
title: Coding An Atom Feed Optimized For Feedly
date: 2018-08-21 19:43:00 -04:00
tags:
- hidden
image: v1535213655/post-images/code-post-image.jpg
readtime: 1
---

<br>
<br>

![Feedly iPhone Mockup](https://res.cloudinary.com/dbrkuvff5/image/upload/f_auto,q_auto/c_scale,q_auto:best,w_250/v1535218675/post-images/iphone-feedly-mockup.jpg){: .width-2 .float-left}

## An Atom Feed Optimized For Feedly That Also Validates
Creating an Atom feed seems like an easy enough task right? Well, in theory it's simple, but like anything worth doing in practice it can be a challenge. 

Before we jump into code, if you're trying to decide between Atom or RSS - either can work fine. I opted to go with Atom because the standard newer, more robust, and designed to do exactly what I'm looking for.

Before we jump into the code here's a few helpful links:
*[The Atom feed for this site](https://markonproduct.com/feed.xml)
*[W3 Validator](https://validator.w3.org/feed/check.cgi?url=https%3A%2F%2Fmarkonproduct.com%2Ffeed.xml)
*[Linked Text](http://url.com)
*[Linked Text](http://url.com)
*[Linked Text](http://url.com)

<hr>

### This is a coded example:


```xml
{% raw %}
<?xml version="1.0" encoding="utf-8"?>
<feed xmlns="http://www.w3.org/2005/Atom" xmlns:webfeeds="http://webfeeds.org/rss/1.0">

<title>{{ site.title }}</title>
<link href="{{ site.url }}/feed.xml" rel="self"/>
<link href="{{ site.url }}/"/>
<updated>{{ site.time | date_to_xmlschema }}</updated>
<id>{{ site.url }}/</id>
<author>
  <name>{{ site.author.name }}</name>
</author>

<webfeeds:cover image="path/to/image.jpg" />
<webfeeds:icon>path/to/image.png</webfeeds:icon>
<webfeeds:logo>path/to/image.svg</webfeeds:logo>
<webfeeds:accentColor>67a43e</webfeeds:accentColor>
<webfeeds:related layout="card" target="browser"/>

{% for post in site.posts %}
  <entry>
   <title>{{ post.title }}</title>
   <link href="{{ site.url }}{{ post.url }}"/>
   <updated>{{ post.date | date_to_xmlschema }}</updated>
   <id>{{ site.url }}{{ post.id }}</id>
   <content type="html">
   {{ post.content | xml_escape }}
   </content>
  </entry>
 {% endfor %}

</feed>
{% endraw %}
```

