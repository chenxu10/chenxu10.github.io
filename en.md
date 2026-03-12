---
layout: default
title: English
permalink: /en/
---

<div class="home">
  <h2 class="post-list-heading">English Posts</h2>
  <ul class="post-list">
    {%- for post in site.posts -%}
      {%- if post.lang == "en" -%}
      <li>
        {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
        <span class="post-meta">{{ post.date | date: date_format }}</span>
        <h3>
          <a class="post-link" href="{{ post.url | relative_url }}">
            {{ post.title | escape }}
          </a>
        </h3>
      </li>
      {%- endif -%}
    {%- endfor -%}
  </ul>
</div>
