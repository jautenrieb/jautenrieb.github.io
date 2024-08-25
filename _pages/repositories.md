---
layout: page
permalink: /repositories/
title: Code
description: Please explore my GitHub account to see some of the projects I've been working on.
nav: true
nav_order: 4
---

{% if site.data.repositories.github_users %}

## GitHub Account

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for user in site.data.repositories.github_users %}
    {% include repository/repo_user.liquid username=user %}
  {% endfor %}
</div>


## GitHub Repositories

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>
{% endif %}
