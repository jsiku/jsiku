---
title: Memos
layout: page
permalink: /memos/
---

{% for memo in site.memos %}
<div>{{memo.content}} {{memo.date | date: '%Y-%m-%d'}}
</div>
{% endfor %}

