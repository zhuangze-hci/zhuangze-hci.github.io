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
  <em>{{ post.venue }}</em>, {{ post.date | date: "%Y" }}.
  {% if post.paperurl %}<a href="{{ post.paperurl }}">Paper</a>{% endif %}
</div>
{% endfor %}

## Academic profiles

- [Google Scholar]({{ site.author.googlescholar }})
- [ORCID]({{ site.author.orcid }})
- [Email](mailto:{{ site.author.email }})
