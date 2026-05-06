---
layout: page
title: professional projects
permalink: /projects/
nav: true
nav_order: 4
---

<div class="projects projects-list">
{% assign sorted_projects = site.projects | sort: "importance" %}
  {% for project in sorted_projects %}
    {% include projects.liquid %}
  {% endfor %}
</div>
