---
layout: default
title: 中文
permalink: /ch/
---

<div class="home">
  <h2 class="post-list-heading">中文文章</h2>
  <ul class="post-list">
    {%- for post in site.posts -%}
      {%- if post.lang == "ch" -%}
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
