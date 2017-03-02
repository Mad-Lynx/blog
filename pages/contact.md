---
layout: page
permalink: /contact/
show_meta: false
title: Contact
published: true
description: "Contact"
comments: false
mathjax: false
noindex: false
tags:
  - address
---

|  |  | 
| :-: | :- |
| <i class="fa fa-paper-plane"></i>  | <{{ site.owner.email }}> | 
|---{% if site.owner.address %}
| <i class="fa fa-envelope"></i> | {{ site.owner.address | newline_to_br | strip_newlines }}   | 
|---
| <i class="fa fa-car"></i>  | [Driving directions](https://www.google.co.uk/maps/dir//{{ site.owner.address | url_encode }}){:target="_blank"} | 
|---{% endif %}{% if site.owner.stackoverflow_id %}
| <i class="fa fa-stack-overflow"></i>  | [StackOverflow](http://stackoverflow.com/users/{{ site.owner.stackoverflow_id }}){:target="_blank"} | 
|---{% endif %}{% if site.owner.github %}
| <i class="fa fa-github"></i>  | [GitHub](https://github.com/{{ site.owner.github }}){:target="_blank"} | 
|---{% endif %}{% if site.owner.linkedin %}
| <i class="fa fa-linkedin"></i>  | [LinkedIn](https://www.linkedin.com/in/{{ site.owner.linkedin }}){:target="_blank"} | 
|---{% endif %}

<a href="javascript:window.print()" class="social-icons" title="Printer friendly format"><i class="fa fa-print"></i></a>

