---
layout: archive
title: "Teaching"
permalink: /teaching/
author_profile: true
---

{% include base_path %}

{% for post in site.teaching reversed %}
  {% if post.was_ta == false %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}

## Teaching Assistant

{% for post in site.teaching reversed %}
  {% if post.was_ta == true %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}