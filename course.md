---
layout: page
title: Course Content
permalink: /course/
---

# 30-Day LLM Mastery Course

Welcome to our comprehensive course on Large Language Models. Below, you'll find links to each day's content.

{% for post in site.posts reversed %}
  {% if post.categories contains "course" %}
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    <p>{{ post.excerpt }}</p>
  {% endif %}
{% endfor %}
