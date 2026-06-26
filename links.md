---
layout: page
title: Official links
permalink: /links/
intro: School, district, committee, and PTO sources that should be used to confirm final decisions.
---

<div class="card-grid">
{% for link in site.data.links %}
<article class="card">
  <p class="eyebrow">{{ link.category }}</p>
  <h2><a href="{{ link.url }}">{{ link.title }}</a></h2>
  <p>{{ link.description }}</p>
</article>
{% endfor %}
</div>
