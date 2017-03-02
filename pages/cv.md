---
layout: page
permalink: /cv/
title: Curriculum Vitae
category: base
published: false
description: "Curriculum Vitae / Resume"
tags:
  - cv
  - resume
comments: false
imagesummary: foo.png
modified: "2016-02-13"
style: |
  .container {
        max-width: 48rem;
    } 
---

{% capture page_title %}{{ page.title }} - {{ site.owner.name }}{% endcapture %}
{% capture print_url %}{{ site.url_assets }}cv.pdf{% endcapture %}
{% capture meta_info %}{% include meta_info.html %}{% endcapture %}{{ meta_info | strip_newlines }}

{:.text-center}

<!-- Alternaetly, user html5 embed tag -->
<iframe src="{{ site.url_assets }}cv.pdf" width="100%" style="height: 100vh;"></iframe>
