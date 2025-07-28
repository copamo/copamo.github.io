---
layout: page
title: Accepted papers
permalink: /papers
order: 3
---

{% assign papers = site.data.papers %}

The tentative list of accepted papers is the following. The list is not final yet as two papers have been conditionally accept.

<div>
  <ul>
    {% for paper in papers %}
      <li><b>{{ paper.title }}</b> by {{ paper.authors }}</li>
    {% endfor %}
  </ul>
</div>
