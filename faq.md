---
layout: page
title: FAQ
permalink: /faq/
intro: A plain-language summary of what is confirmed, proposed, or still unknown.
---

<div class="stack">
{% for item in site.data.faq %}
<article class="card">
  <span class="status status-{{ item.status_key }}">{{ item.status }}</span>
  <h2>{{ item.question }}</h2>
  <p>{{ item.answer }}</p>
  {% if item.source_url and item.source_url != "" %}
  <p><a href="{{ item.source_url }}">Official source</a></p>
  {% endif %}
  <p class="small">Last updated: {{ item.updated }}</p>
</article>
{% endfor %}
</div>
