---
title: Memos
layout: page
permalink: /memos/
---

{% for post in site.memos %}
<p>{{post.content}}
{{post.date | date: '%F'}}
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

