---
layout: default
title: GitHub Projects
permalink: /github-projects/
---

# GitHub Projects

A selection of side projects I built during my intensive MERN stack coding bootcamp. Each showcases different aspects of my learning journey.  

✅ ~~**Phase 2:** Rebuild this portfolio using Jekyll and GitHub Pages.~~  
🚀 **Phase 3:** Add more recent personal projects and open-source work.


<div class="gh-grid" markdown="0">
{% for p in site.data.github_projects %}
<article class="gh-card gh-card--row">
    <a class="gh-thumb" href="{{ p.repo }}" target="_blank" rel="noopener">
      <img src="{{ p.img | relative_url }}" alt="{{ p.title }} thumbnail">
    </a>
    <div class="gh-body">
      <div class="gh-headline">
        <h3 class="gh-title">{{ p.title }}</h3>
        {% if p.kind %}<span class="gh-kind">{{ p.kind }}</span>{% endif %}
      </div>
      <p class="gh-blurb">{{ p.blurb }}</p>
      <p class="gh-links">
        <a class="learn-link" href="{{ p.repo }}" target="_blank" rel="noopener">View repository →</a>
      </p>
    </div>
  </article>
{% endfor %}
</div>
