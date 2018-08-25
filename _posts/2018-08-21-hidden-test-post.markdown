---
title: Coding An Atom Feed Optimized For Feedly
date: 2018-08-21 19:43:00 -04:00
tags:
- hidden
image: v1535213655/post-images/code-post-image.jpg
readtime: 1
---

## Sub-Headline



![Feedly iPhone Mockup](https://res.cloudinary.com/dbrkuvff5/image/upload/v1535218675/post-images/iphone-feedly-mockup.jpg){: .width-2 .float-left}


Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur imperdiet lobortis viverra. Phasellus eu felis urna. Morbi molestie urna urna, vitae fermentum lacus euismod quis. Nunc rutrum posuere tristique. Vestibulum consequat ac nunc eget blandit. Curabitur ultricies diam vitae sem bibendum semper. Aenean finibus gravida lobortis.

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur imperdiet lobortis viverra. Phasellus eu felis urna. Morbi molestie urna urna, vitae fermentum lacus euismod quis. Nunc rutrum posuere tristique. Vestibulum consequat ac nunc eget blandit. Curabitur ultricies diam vitae sem bibendum semper. Aenean finibus gravida lobortis.


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

 <webfeeds:cover image="https://res.cloudinary.com/dbrkuvff5/image/upload/v1534161359/post-images/mark-on-product.jpg" />
 <webfeeds:icon>https://res.cloudinary.com/dbrkuvff5/image/upload/v1534497630/assets/favicon-96x96.png</webfeeds:icon>
 <webfeeds:logo>https://res.cloudinary.com/dbrkuvff5/image/upload/v1534707051/assets/logo-reversed.svg</webfeeds:logo>
 <webfeeds:accentColor>67a43e</webfeeds:accentColor>
 <webfeeds:related layout="card" target="browser"/>

 {% for post in site.posts %}
 <entry>
   <title>{{ post.title }}</title>
   <link href="{{ site.url }}{{ post.url }}"/>
   <updated>{{ post.date | date_to_xmlschema }}</updated>
   <id>{{ site.url }}{{ post.id }}</id>
   <content type="html">
   	&lt;img class=&quot;post-image&quot; alt=&quot;Article Image&quot; src=&quot;https://res.cloudinary.com/dbrkuvff5/image/upload/f_auto/c_scale,q_auto:good,w_845/{{ post.image | xml_escape }}&quot;&gt;
   {{ post.content | xml_escape }}
   </content>
 </entry>
 {% endfor %}

</feed>
{% endraw %}
```

