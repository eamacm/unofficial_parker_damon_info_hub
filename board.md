---
layout: page
title: PTO board and organizing roles
permalink: /board/
intro: Publicly announced or consented-to board and interim organizing roles.
---

<div class="notice">
Names should be added only when the person has agreed to be listed or the role has been publicly announced through an official source.
</div>

<div class="card-grid">
{% for person in site.data.board %}
<article class="card">
  <span class="status status-{{ person.status_key }}">{{ person.status }}</span>
  <h2>{{ person.role }}</h2>
  <p class="person-name">{{ person.name }}</p>
  {% if person.note %}<p>{{ person.note }}</p>{% endif %}
</article>
{% endfor %}
</div>
