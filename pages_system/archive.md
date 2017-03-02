---
layout: page
title: Archive
description: "Archive"
permalink: /archive/
category: base
---

{% capture site_year %}{{ site.time | date: '%Y' }}{% endcapture %}
<section id="archive">
  {%for post in site.posts %}
    {% capture year %}{{ post.date | date: '%Y' }}{% endcapture %}
    {% unless post.next %}
      <h3>{% if site_year == year %}This year's posts{% else %}{{ post.date | date: '%Y' }}{% endif %}</h3>
      <ul class="post-list">
    {% else %}
      {% capture nyear %}{{ post.next.date | date: '%Y' }}{% endcapture %}
      {% if year != nyear %}
        </ul>
        <h3>{{ post.date | date: '%Y' }}</h3>
        <ul class="post-list">
      {% endif %}
    {% endunless %}
      <li><a href="{{ site.url }}{{ post.url }}">{{ post.title }}<span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%b %d, %Y" }}</time></span></a></li>
  {% endfor %}
  </ul>
</section>
