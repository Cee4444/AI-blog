---
layout: default
title: Home
---

# Blog Home Page

Welcome to my website where I post blogs that discuss different trending topcis on technonlogy and other surrounding fields. 
Here are my latest posts:

---

<ul>
  {% assign pages_list = site.pages | where_exp:"p","p.path contains 'posts'" | sort: "date" | reverse %}
  {% for page in pages_list %}
    <li>
      <a href="{{ page.url | relative_url }}">{{ page.title }}</a><br>
      {% if page.date %}
      <small>{{ page.date | date: "%B %d, %Y" }}</small>
      {% endif %}
    </li>
  {% endfor %}
</ul>

---

✨ Thank you for coming to my website — I intend to keep adding new blogs, projects and reports here. ✨
