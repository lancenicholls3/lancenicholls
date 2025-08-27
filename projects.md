---
layout: single
title: "Projects"
permalink: /projects/
---

Below are selected engineering projects.

{% assign posts = site.projects | sort: 'date' | reverse %}
<ul>
{% for p in posts %}
  <li>
    <a href="{{ p.url | relative_url }}"><strong>{{ p.title }}</strong></a>
    — {{ p.subtitle | default: p.summary | default: p.excerpt }}
  </li>
{% endfor %}
</ul>
