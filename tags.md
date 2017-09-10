---
title: Tags
layout: page
permalink: /tags/
published: true
---

<ul>
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


{% for tag in site.tags %}
 
 {% unless tag.first == 'memo' %}
    {% capture tag_name %}{{ tag | first }}{% endcapture %}
    <h4 id="#{{ tag_name | slugize }}">{{ tag_name }}</h4>
    <a name="{{ tag_name | slugize }}"></a>
{% endunless %}
    {% for post in site.tags[tag_name] %}
    <article class="archive-item">
      <h5><a href="{{site.baseurl}}{{ post.url }}">{{post.title}}</a></h5>
    </article>
    {% endfor %}
 
{% endfor %}

