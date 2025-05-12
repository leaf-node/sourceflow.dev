---
title: Donate
layout: page
---

<div>
    {% for social in site.sociallinks %}
    {% if social.name == "buymeacoffee" %}
        <p>Let's <a rel="me" href="{{ social.url }}">donate</a>!</p>
    {% endif %}
    {% endfor %}
</div>

