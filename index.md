---
layout: default
title: Home
---

# Power & Grace Performance: Maddisen

Here are my Markdown files:

{% for page in site.pages %}
  {% if page.name != 'index.md' and page.name != '404.html' %}
  - [{{ page.title | default: page.name }}]({{ page.url }})
  {% endif %}
{% endfor %}
