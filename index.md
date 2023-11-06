---
layout: default
---

# Welcome to my page

Here's a list of my projects:
{% for project in site.projects %}
  - [{{ project.title }}]({{ project.link }}): {{ project.content | strip_html | strip_newlines | truncate: 160 }}
{% endfor %}
