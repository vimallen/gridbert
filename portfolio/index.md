---
title: Portfolio
author: Dave Allen
layout: portfolio
permalink: /portfolio/
---

{% for job in site.data.jobs %}

<div class="module-portfolio">
<h3>{{job.name}}</h3>
<a href="{{job.link}}" class="what"><img src="{{job.image}}"></a>
<p>Client: {{job.client}}</p>
<p>Description: {{job.description}}</p>
<p><a href="{{job.link}}">Read more &#8230;</a></p>
</div>

{% endfor %}
