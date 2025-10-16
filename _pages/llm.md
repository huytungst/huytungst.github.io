---
title: "Large Language Models (LLM)"
permalink: /LLM/
layout: collection
collection: posts
entries_layout: grid
classes: wide
---

Welcome to the Large Language Models section! Here you'll find posts and articles related to LLMs, transformers, natural language processing, and generative AI.

{% assign llm_posts = site.posts | where: "categories", "LLM" %}
{% if llm_posts.size > 0 %}
<div class="feature__wrapper">
  {% for post in llm_posts %}
    {% include archive-single.html type="grid" %}
  {% endfor %}
</div>
{% else %}
<p>No LLM posts yet. Check back soon for exciting content!</p>
{% endif %}