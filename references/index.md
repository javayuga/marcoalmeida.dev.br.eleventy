---
layout: layouts/post.njk
title: References
templateClass: tmpl-post
eleventyNavigation:
  key: References
  order: 3
---

[Markdown Cheat Sheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

{% set navPages = collections.all | eleventyNavigation("References") %}
<ol reversed class="postlist">
{% for navPage in navPages%}
  <li class="postlist-item">
    <a href="{{ navPage.url | url }}" class="postlist-link"> {{ navPage.key }}</a>
  </li>
{% endfor %}
</ol>
