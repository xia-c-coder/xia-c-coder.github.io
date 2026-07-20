---
layout: default
title: 首页
---

<h1>📝 最新文章</h1>

<ul>
  {% for post in site.posts %}
    <li style="margin-bottom: 10px;">
      <a href="{{ post.url }}" style="font-size: 18px;">{{ post.title }}</a>
      <span style="color: #666; margin-left: 15px;">{{ post.date | date: "%Y-%m-%d" }}</span>
    </li>
  {% endfor %}
</ul>
