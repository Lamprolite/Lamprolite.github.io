---
layout: blog
title: Study
slug: /study
---

{% assign study_posts = site.posts | where_exp: "post", "post.categories contains 'study'" %}
<ul>
  {% for post in study_posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a> - {{ post.date | date: "%Y-%m-%d" }}
    </li>
  {% endfor %}
</ul>
