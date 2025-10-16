---
title: "Machine Learning"
permalink: /ML/
layout: collection
collection: posts
entries_layout: grid
classes: wide
---

Welcome to the Machine Learning section! Here you'll find posts and articles related to Machine Learning concepts, algorithms, and applications.

{% assign ml_posts = site.posts | where: "categories", "Machine Learning" %}
{% if ml_posts.size > 0 %}
<div class="feature__wrapper">
  {% for post in ml_posts %}
    {% include archive-single.html type="grid" %}
  {% endfor %}
</div>
{% else %}
<p>No Machine Learning posts yet. Check back soon for exciting content!</p>
{% endif %}