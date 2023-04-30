---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% if post.inprogress == false %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}

## Publications In Progress

{% for post in site.publications reversed %}
  {% if post.inprogress == true %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}