---
layout: layout.liquid
title: Hello frontmatter!
pagination:
  data: collections.blog
  size: 2
  alias: blogs
---
Welcome to my site!

## Latest blog posts

{% for blog in blogs %}

- [{{blog.data.title}}]({{blog.url}})

{% endfor %}

{% if pagination.href.previous %}
  <a href="{{pagination.href.previous}}">Previous Page</a>
{% endif %}
{% if pagination.href.next %}
  <a href="{{pagination.href.next}}">Next Page</a>
{% endif %}
