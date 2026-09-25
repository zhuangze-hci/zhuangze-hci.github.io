---
permalink: /
title: ""
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<section class="profile-intro">
  <p class="profile-kicker">Human-Computer Interaction · Human-AI Interaction · MR/VR</p>
  <h1>Hou Zhuangze</h1>
  <p class="profile-lead">
    I am a Ph.D. Candidate in Creative Media at the School of Creative Media,
    City University of Hong Kong. My research sits at the intersection of
    human-computer interaction, human-AI interaction, and mixed and virtual reality.
  </p>
  <p>
    I design and study interactive systems that help people communicate spatial
    intent, author immersive environments, and collaborate with AI in transparent
    and controllable ways.
  </p>
  <div class="profile-actions">
    <a class="profile-button profile-button--primary" href="/publications/">View publications</a>
    <a class="profile-button" href="/cv/">View CV</a>
    <a class="profile-button" href="mailto:zhuanghou3-c@my.cityu.edu.hk">Email me</a>
  </div>
</section>

## Research interests

<div class="research-tags" aria-label="Research interests">
  <span>Human-Computer Interaction</span>
  <span>Human-AI Interaction</span>
  <span>Mixed Reality</span>
  <span>Virtual Reality</span>
  <span>Spatial Interaction</span>
</div>

## Featured publications

{% assign sorted_publications = site.publications | sort: "date" | reverse %}
{% for post in sorted_publications limit:2 %}
  {% include publication-card.html post=post %}
{% endfor %}

<p class="section-link"><a href="/publications/">See all publications →</a></p>
