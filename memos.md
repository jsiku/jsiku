---
title: Memos
layout: page
permalink: /memos/
---

{% for memo in site.memos %}
<p>{{memo.content}}
{{memo.date | date: '%Y-%m-%d'}}
    {% assign tags = memo.tags %}
  {% for tag in tags %}
  <code><a href="{{site.baseurl}}/tags/#{{tag|slugize}}">{{tag}}</a></code>
  {% endfor %}

</p>
{% endfor %}

