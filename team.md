---
layout: page
title: Our Team
permalink: /team/
---

{% for member in site.data.team %}
  <div class="teammember">
  <p> {{ member.name }} </p>
  <p> {{ member.description }} </p>
  {% if member.github %}
    {% include icon-github.html username=member.github label='GitHub' %}
  {% endif %}
  {% if member.linkedin %}
    {% include icon-linkedin.html username=member.linkedin label='Linkedin' %}
  {% endif %}
  </div>

{% if forloop.last %}{% else %}<br>{% endif %}
{% endfor %}
