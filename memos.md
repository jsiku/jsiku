---
title: Memos
layout: page
permalink: /memos/
published: true
---

{% for post in site.memos reversed %}

<p>{{post.content}}
{{post.date | date: '%F'}}
{% if post %}
    {% assign tags = post.tags %}
  {% else %}
    {% assign tags = page.tags %}
  {% endif %}
  {% for tag in tags %}
  {% unless tag == 'memo' %}
  <code><a href="{{site.baseurl}}/tags/#{{tag|slugize}}">{{tag}}</a></code>
  {% endunless %}
   {% endfor %}

</p>

{% endfor %}
