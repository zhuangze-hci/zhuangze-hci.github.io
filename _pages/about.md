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
    of Prof. Can Liu. I am currently a visiting scholar at Singapore Management
    University, working with Prof. Jiannan Li.
  </p>
  <p>
    Before beginning my Ph.D., I received both my bachelor's and master's degrees
    in Software Engineering from Dalian University of Technology. During my
    master's studies, I conducted research under the supervision of Prof. Qiufen Xia.
  </p>
  <p>
    My research explores how AI can support immersive creation beyond one-shot
    generation. I develop multimodal, context-aware systems that use AI to interpret
    underspecified goals, integrate speech, gesture, embodied and scene context, and
    maintain interaction history across turns. By externalizing AI-generated
    suggestions, spatial references, uncertainty, and constraints as inspectable
    intermediate representations, my work helps users explore alternatives and
    translate evolving intent into reversible and executable actions. Across VR, MR,
    and situated physical making, I investigate how AI can provide adaptive creative
    and spatial assistance while keeping people in control of decisions and outcomes.
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
