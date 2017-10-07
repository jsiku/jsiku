---
title: Memos
layout: page
permalink: /memos/
---

{% for post in site.memos %}
<p>{{post.content}}
{{post.date | date: '%Y-%m-%d'}}
{% if post %}
    {% assign tags = post.tags %}
  {% else %}
    {% assign tags = page.tags %}
  {% endif %}
  {% for tag in tags %}
  <code><a href="{{site.baseurl}}/tags/#{{tag|slugize}}">{{tag}}</a></code>
  {% endfor %}

</p>
{% endfor %}

