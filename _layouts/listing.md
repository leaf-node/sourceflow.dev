---
layout: default
---

<h1>{{ page.title }}</h1>

<ul class="listing">
{% for p in site.pages %}
   {% if p.categories contains page.category %}
     <li>
        <a href="{{ p.url | absolute_url }}">
          <img src="{{ p.image | absolute_url }}" \>
          <h2>{{ p.title }}</h2>
          <p class="dark">{{ page.author | default: site.author }}</p>
          <p class="summary">{{ p.content | strip_html | truncatewords: 50 }}</p>
        </a>
      </li>
   {% endif %}
{% endfor %}
</ul>
