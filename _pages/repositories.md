---
layout: page
permalink: /repositories/
title: Repositories
description: Here's a list of some of my recent Github repositories. See my github page for detailed information and more repositories.
nav_order: 3
nav: true
---

{% if site.data.repositories.github_repos %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.html repository=repo %}
  {% endfor %}
</div>
{% endif %}
