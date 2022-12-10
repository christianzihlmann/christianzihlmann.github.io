---
layout: archive
title: "Research"
permalink: /publications/
author_profile: true
---

<h1>Articles (peer-reviewed)</h1>
{% for post in site.publications reversed %}
  {% if post.pubtype == 'journal' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}

<h2><i>Working Papers</i></h2>
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