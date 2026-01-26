{% assign paper = papers | where_exp: "p", "p.paperid == talk.paperid" | first %}
{% assign start = talk.start %}
{% assign end = talk.end %}
{% assign title = paper.title %}
{% assign authors = paper.authors %}
{% assign url = paper.url %}
{% assign slides = paper.slides %}

<li>
  {{start}}-{{end}}&nbsp;&nbsp;
  <i>
    {% if url %}
      <a href="{{ url | relative_url }}">{{ title }}</a>
    {% else %}
      {{ title }}
    {% endif %}
  </i> by {{ authors }}
  {% if slides %}
    &nbsp;[<a href="{{ slides }}">slides</a>]
  {% endif %}
</li>
