---
layout: page
permalink: /repositories/
title: repositories
description: Selected open-source projects and repositories on GitHub.
nav: true
nav_order: 4
---

<style>
  .static-repositories {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 1.25rem;
    margin: 1.5rem 0 2rem;
  }

  .static-repository-card {
    border: 1px solid var(--global-divider-color);
    border-radius: 8px;
    padding: 1.25rem;
    min-height: 160px;
    background: var(--global-card-bg-color, transparent);
  }

  .static-repository-card h3 {
    margin: 0 0 0.75rem;
    font-size: 1.25rem;
  }

  .static-repository-card h3 a {
    color: var(--global-theme-color);
  }

  .static-repository-card p {
    min-height: 3rem;
    margin-bottom: 1.25rem;
  }

  .static-repository-language {
    color: var(--global-text-color-light);
    font-size: 0.95rem;
  }
</style>

<h2 id="github-repositories">GitHub Repositories</h2>

<div class="static-repositories">
  {% for repository in site.data.repositories.static_repositories %}
    <article class="static-repository-card">
      <h3>
        <a href="{{ repository.url }}" rel="external nofollow noopener" target="_blank">{{ repository.name }}</a>
      </h3>
      <p>{{ repository.description }}</p>
      <span class="static-repository-language">{{ repository.language }}</span>
    </article>
  {% endfor %}
</div>
