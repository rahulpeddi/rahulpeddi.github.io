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

{% assign ordered_pages = site.publications | sort:"order_number" %}

{% for post in ordered_pages reversed %}
  {% include archive-single.html %}
{% endfor %}
