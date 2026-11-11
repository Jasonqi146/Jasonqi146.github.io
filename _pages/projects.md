---
layout: page
title: Projects
nav_title: Projects
description: Infrastructure for agent training, evaluation, and scalable oversight.
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
