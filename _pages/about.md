---
permalink: /
title: "汽车资讯小站"
excerpt: "最新汽车资讯"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

# 欢迎来到汽车资讯小站

这里收录最新的汽车资讯、车型评测和行业动态。

## 最新文章

{% for post in site.posts limit:5 %}
  <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
  <p>{{ post.date | date: "%Y-%m-%d" }} | {{ post.excerpt | strip_html | truncate: 200 }}</p>
{% endfor %}
