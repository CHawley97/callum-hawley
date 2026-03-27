---
layout: default
title: Home
---

# Welcome to my Portfolio

This is my custom-built site using Jekyll.

## My Latest Articles
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </li>
  {% else %}
    <li>No posts found in the _posts folder!</li>
  {% endfor %}
</ul>