---
layout: page
title: projects
permalink: /projects/
description: Representative systems work across open source, search, infrastructure, and applied machine learning.
nav: true
nav_order: 3
---

<div class="collection-intro">
  <p>
    These projects are not a full picture of my recent research work, but they show a recurring pattern in how I build: turning ideas
    into reliable systems with clear interfaces, evaluation, and iteration loops.
  </p>
</div>

<div class="projects projects-list">
{% assign sorted_projects = site.projects | sort: "importance" %}
  {% for project in sorted_projects %}
    {% include projects.liquid %}
  {% endfor %}
</div>
