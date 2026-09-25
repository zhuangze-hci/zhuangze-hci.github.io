---
permalink: /
title: ""
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<section class="profile-intro">
  <p class="profile-kicker">Human-AI Interaction · Multimodal Interaction · Immersive Creation</p>
  <h1>About me</h1>
  <p class="profile-lead">
    I am a second-year Ph.D. candidate in Human-Computer Interaction (HCI) at the
    School of Creative Media, City University of Hong Kong, under the supervision
    of Professor Can Liu.
  </p>
  <p>
    My research focuses on AI-assisted multimodal interaction for immersive creation.
    I study how people express and progressively refine underspecified creative and
    spatial intentions through speech, gesture, embodied context, scene information,
    and interaction history. I design transparent and repairable mixed-initiative
    systems that help people turn these evolving intentions into controllable actions
    across VR, MR, and situated physical making, while preserving human agency
    throughout the process.
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
  <span>Multimodal Interaction</span>
  <span>VR/MR</span>
  <span>Immersive Creation</span>
</div>

## Featured publications

{% assign sorted_publications = site.publications | sort: "date" | reverse %}
{% for post in sorted_publications limit:2 %}
  {% include publication-card.html post=post %}
{% endfor %}

<p class="section-link"><a href="/publications/">See all publications →</a></p>
