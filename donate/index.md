---
title: Donate
layout: page
---

<div class="sociallinks">
    {% for social in site.sociallinks %}
    {% if social.name == "buymeacoffee" %}
        <a rel="me" href="{{ social.url }}"><img src="{{ "/assets/img/social/" | absolute_url }}{{ social.icon }}"/> Buy Andrew a coffee</a>
    {% endif %}
    {% endfor %}
</div>

