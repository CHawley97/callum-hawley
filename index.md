---
layout: default
title: Home
---

# Welcome to my Portfolio

This is my custom-built site using Jekyll. Here is what I've been writing lately:

## Latest Posts
<ul>
  {% for post in site.posts %}
    <li>
      <span class="post-date">{{ post.date | date: "%b %-d, %Y" }}</span>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>

---

### About this site
Built with HTML, CSS, and Jekyll. [Read more about me]({{ '/about/' | relative_url }})