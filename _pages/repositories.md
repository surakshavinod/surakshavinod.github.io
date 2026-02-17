---
layout: page
permalink: /repositories/
title: repositories
description: find some of my GitHub repos here!
nav: true
nav_order: 3
---

{% if site.data.repositories.github_repos %}

<div class="row">
  {% for repo in site.data.repositories.github_repos %}
    <div class="col-12 col-sm-6 col-md-4 mb-4 d-flex">
      {% include repository/repo.liquid repository=repo %}
    </div>
  {% endfor %}
</div>

{% endif %}


