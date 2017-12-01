---
layout: page
title: Data Science Cheat Sheets
permalink: /teachingresources/
---

Find here some useful cheat sheets for your Data Science learning efforts.

Be sure to check back, we will be adding many more!

<div class="resource_grid">

{% for resource in site.data.teachingresources %}

  {% if resource.internal %} 

  <div class="internal_resource">
  <h3>   <a href="{{ resource.path }}"> {{ resource.name }} </a></h3>

  <p> {{ resource.description | markdownify }} </p>
  </div>
  {% endif %}
{% endfor %}
</div>
