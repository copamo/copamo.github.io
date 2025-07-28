---
layout: page
title: Accepted papers
permalink: /papers
order: 3
---

{% assign papers = site.data.papers %}

<div>
	<ul>
		{% for paper in papers %}
      <li>"<i>{{ paper.title }}</i>" by {{ paper.authors }}</li>
		{% endfor %}
	</ul>
</div>
