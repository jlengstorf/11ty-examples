---
layout: layout.liquid
title: Home
---
Welcome to my site!

## Latest blog posts

{% for blog in collections.blog %}

- [{{blog.data.title}}]({{blog.url}})

{% endfor %}
