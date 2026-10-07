---
layout: default
title: Home
---
Welcome! This site is my writeup on **[your topic]**, built with a Python notebook, NotebookLM, and Jekyll.

[About me]({{ '/about/' | relative_url }})

## Posts

{% for post in site.posts %}
- [{{ post.title }}]({{ post.url | relative_url }}) ({{ post.date | date: "%B %-d, %Y" }})
{% endfor %}
