---
layout: page
title: Accepted papers
permalink: /papers
order: 3
---

{% assign papers = site.data.papers %}

The tentative list of accepted papers is the following.

The is not the final list yet as some papers have been conditionally accepted. If your paper has been conditionally accepted, you will receive detailed instructions to proceed.

<div>
  <ul>
    {% for paper in papers %}
      <li><b>{{ paper.title }}</b> by {{ paper.authors }}</li>
    {% endfor %}
  </ul>
</div>
