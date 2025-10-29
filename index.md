---
layout: default
title: Home
---

# Blog Home Page

Welcome to my website where i post blogs that discuss different trending topcis on technonlogy and other surrounding fields. 
Here are my latest posts:

---

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a><br>
      <small>{{ post.date | date: "%B %d, %Y" }}</small>
    </li>
  {% endfor %}
</ul>

---

✨ Thank you for coming to my website — I intend to keep adding new blogs, projects and reports here. ✨
