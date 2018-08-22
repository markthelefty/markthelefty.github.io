---
title: Archive
date: 2018-08-05 13:43:00 -04:00
---

<section class="post">

   {% for post in site.posts %}
{% unless post.tags contains 'hidden' %}
       {% assign currentDate = post.date | date: "%Y" %}
       {% if currentDate != myDate %}
           {% unless forloop.first %}</ul>{% endunless %}
           <h2>{{ currentDate }}</h2>
           <ul>
           {% assign myDate = currentDate %}
       {% endif %}
       <li><a href="{{ post.url }}"><span>{{ post.date | date: "%B %-d, %Y" }}</span> - {{ post.title }}</a></li>
       {% if forloop.last %}</ul>{% endif %}
   {% endunless %}
   {% endfor %}

</section>