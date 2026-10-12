---
layout: page
title: Tags
permalink: /tags/
---

{%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
{%- assign tags = site.tags | sort -%}
{%- for tag in tags %}
<h2 id="{{ tag[0] | slugify }}">#{{ tag[0] }}</h2>
<ul class="tag-post-list">
  {%- for post in tag[1] %}
  <li>
    <span class="post-meta">{{ post.date | date: date_format }}</span>
    <a href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
  </li>
  {%- endfor %}
</ul>
{%- endfor %}
