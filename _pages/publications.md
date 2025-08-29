---
layout: archive
# title: "Research"
permalink: /publications/
author_profile: true
---

<h1>Articles (peer-reviewed)</h1>
{% for post in site.publications reversed %}
  {% if post.pubtype == 'journal' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}
<br>
<h1>Working Papers</h1>
{% for post in site.publications reversed %}
  {% if post.pubtype == 'workingpaper' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}
<br>
<h1>Other research contributions</h1>
{% for post in site.publications reversed %}
  {% if post.pubtype == 'other' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}
<br>
<h1>Work in progress</h1>
{% for post in site.publications reversed %}
  {% if post.pubtype == 'wip' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}
