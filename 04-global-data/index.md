---
layout: layout.liquid
title: Hello frontmatter!
---
Welcome to my site!

## Latest blog posts

{% for blog in collections.blog %}

- [{{blog.data.title}}]({{blog.url}})

{% endfor %}
