---
layout: page
title: Our Team
permalink: /team/
---

{% for member in site.data.team %}
  <div class="teammember">
  
  <h3> {{ member.name }} </h3>
  
  <p> {{ member.description }} </p>
  
  {% if member.github %}
    {% include icon-github.html username=member.github label='GitHub' %}
  {% endif %}
  
  <div class="horizontalgap" style="width:10px"></div>
  {% if member.linkedin %}
    {% include icon-linkedin.html username=member.linkedin label='LinkedIn' %}
  {% endif %}
  
  <div class="horizontalgap" style="width:10px"></div>
  {% if member.website %}
    <a href="http://{{ member.website }}">Personal Website</a>
  {% endif %}
  </div>

{% if forloop.last %}{% else %}<br>{% endif %}
{% endfor %}
