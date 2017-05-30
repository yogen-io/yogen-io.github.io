---
layout: page
title: Our Team
permalink: /team/
---

{% for member in site.data.team %}
<div class="teammember">
<p> {{ member.name }} </p>
<p> {{ member.description }} </p>
</div>
{% endfor %}
