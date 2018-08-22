---
title: Archive
date: 2018-08-05 13:43:00 -04:00
---

<section class="post">
   {% for post in site.posts %}
       {% assign currentDate = post.date | date: "%Y" %}
       {% if currentDate != myDate %}
           {% unless forloop.first %}</ul>{% endunless %}
           <h2>{{ currentDate }}</h2>
           <ul>
           {% assign myDate = currentDate %}
       {% endif %}
        {% unless post.tags contains 'hidden' %}
          <li><a href="{{ post.url }}"><span>{{ post.date | date: "%B %-d, %Y" }}</span> - {{ post.title }}</a></li>
        {% endunless %}
       {% if forloop.last %}</ul>{% endif %}
   {% endfor %}
</section>