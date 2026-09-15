---
layout: default
title: "Laís Carneiro"
description: "Invasion ecologist working on how to classify, measure and compare the ecological impacts of invasive species."
---

<div class="shell hero">
  <div>
    <h1 class="hero__name">Laís Carneiro</h1>
    <p class="hero__role">
      <strong>Postdoctoral researcher in invasion ecology.</strong>
      ESE lab, Université Paris-Saclay — Franck Courchamp's group.
    </p>
    <ul class="profiles">
      <li><a href="https://scholar.google.com/citations?user=rUvrtAsAAAAJ" target="_blank" rel="noopener">Google Scholar</a></li>
      <li><a href="https://orcid.org/0000-0002-3828-7751" target="_blank" rel="noopener">ORCID</a></li>
      <li><a href="https://github.com/lalacarneiro" target="_blank" rel="noopener">GitHub</a></li>
      <li><a href="https://www.researchgate.net/profile/Lais-Carneiro" target="_blank" rel="noopener">ResearchGate</a></li>
      <li><a href="https://www.linkedin.com/in/laiscarneiro/" target="_blank" rel="noopener">LinkedIn</a></li>
    </ul>
  </div>
  <figure class="portrait">
    <img src="{{ '/assets/images/portrait.jpg' | relative_url }}"
         alt="Laís Carneiro standing on a ridge in the Atlas mountains, Morocco"
         width="900" height="1125">
  </figure>
</div>

<section class="shell section">
  <div class="section__lead">
    <h2>What I work on</h2>
    <p>
      How much damage does an invasive species actually do? The question sounds
      simple and isn't. Impacts are reported across thousands of separate studies,
      in units that don't line up, for a small set of well-studied species — which
      makes them very hard to compare, and harder still to act on.
    </p>
    <p>
      My research turns that scattered evidence into something standardised. I build
      typologies and severity scales for ecological impact, run global syntheses and
      meta-analyses, and design metrics that let impacts be ranked across species,
      habitats and continents. I trained as an environmental engineer before moving
      into ecology, and I still work that way: measurement first, then inference.
    </p>
    <p><a href="{{ '/research.html' | relative_url }}">More about the research</a></p>
  </div>
</section>

<section class="shell section">
  <h2>Recent papers</h2>
  {% assign recent = site.data.publications | slice: 0, 3 %}
  {% for pub in recent %}
    {% include publication.html pub=pub %}
  {% endfor %}
  <p><a href="{{ '/publications.html' | relative_url }}">All publications</a></p>
</section>
