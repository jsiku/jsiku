---
title: Tags
layout: page
permalink: /tags/
published: true
---

<ul class="tag-cloud">
{% for tag in site.tags %}
  <span style="font-size: {{ tag | last | size | times: 100 | divided_by: site.tags.size | plus: 70  }}%">
{% unless tag.first == 'memo' %}
    <a href="#{{ tag | first | slugize }}">
      {{ tag | first }}
    </a> &nbsp;&nbsp;
    {% endunless %}
  </span>
{% endfor %}
</ul>

<div id="archives">
{% for tag in site.tags %}
  <div class="archive-group">
{% unless tag.first == 'memo' %}
    {% capture tag_name %}{{ tag | first }}{% endcapture %}
    <h3 id="#{{ tag_name | slugize }}">{{ tag_name }}</h3>
    <a name="{{ tag_name | slugize }}"></a>
{% endunless %}
    {% for post in site.tags[tag_name] %}
    <article class="archive-item">
      <h4><a href="{{site.baseurl}}{{ post.url }}">{{post.title}}</a></h4>
    </article>
    {% endfor %}
  </div>
{% endfor %}
</div>
