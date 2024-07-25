---
layout: home
title: "Home"
---

Welcome to my site!

## Recent Malware Analysis Posts

{% for post in site.malware_analysis %}
  * [{{ post.title }}]({{ post.url }})
{% endfor %}

## Recent Application Pentesting Posts

{% for post in site.application_pentesting %}
  * [{{ post.title }}]({{ post.url }})
{% endfor %}
