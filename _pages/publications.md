---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

<h2>Articles (peer-reviewed)</h2>
{% for post in site.publications reversed %}
  {% if post.pubtype == 'journal' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}

<h2>Working Papers</h2>
{% for post in site.publications reversed %}
  {% if post.pubtype == 'workingpaper' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}

<h2>Work in progress</h2>
{% for post in site.publications reversed %}
  {% if post.pubtype == 'wip' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}