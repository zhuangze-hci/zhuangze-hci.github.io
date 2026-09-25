---
layout: archive
title: "Curriculum Vitae"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

## Current position

**Ph.D. Candidate in Creative Media**<br>
School of Creative Media, City University of Hong Kong

**Visiting Scholar**<br>
Singapore Management University — working with Prof. Jiannan Li

## Research interests

- Human-Computer Interaction
- Human-AI Interaction
- Mixed Reality and Virtual Reality
- Multimodal and spatial interaction
- AI-assisted immersive authoring

## Publications

{% assign sorted_publications = site.publications | sort: "date" | reverse %}
{% for post in sorted_publications %}
<div class="cv-publication">
  <strong>{{ post.title }}</strong><br>
  {{ post.authors }}<br>
  {% if post.contribution_note %}<span class="publication-card__note">{{ post.contribution_note }}</span><br>{% endif %}
  <em>{{ post.venue }}</em>, {{ post.date | date: "%Y" }}.
  {% if post.paperurl %}<a href="{{ post.paperurl }}">Paper</a>{% endif %}
</div>
{% endfor %}

## Academic profiles

- [Google Scholar]({{ site.author.googlescholar }})
- [ORCID]({{ site.author.orcid }})
- [Email](mailto:{{ site.author.email }})
