---
layout: default
title: "EEICAT: summary and references"
heading: "EEICAT: summary and references"
subheading: "Summary, key terms and references accompanying the talk on extending invasive species impact assessments to the ecosystem level. Recommended starting points are marked with a vertical line."
description: "Summary, key terms and references on EEICAT, the Extended Environmental Impact Classification for Alien Taxa, and on the ecological impacts of biological invasions."
permalink: /talks/eeicat.html
---

{% assign sections = site.data.eeicat_reading %}

<section class="shell section" style="border-top:0; padding-top:0">
  <div class="section__lead">
    <h2>Summary</h2>
    <p>
      EICAT is the IUCN standard for classifying how severe the environmental
      impacts of an alien species are, from Minimal Concern to Massive. It works
      well, but it looks almost only at what happens to native species. Of the 19
      types of ecological impact we identified in the literature, it covers 7.
    </p>
    <p>
      EEICAT (Extended EICAT) keeps the EICAT logic and severity scale and adds
      the other 12. Impacts are grouped in three dimensions: individuals and
      populations, species and communities, and ecosystems and the abiotic
      environment, such as nutrient cycling, water quality or fire regimes.
    </p>
    <p>
      The other change is the unit of assessment. EICAT gives each species one
      global score; EEICAT scores an invasion event, so the same species can have
      a different impact profile in each place it invades. Existing impact studies
      and EICAT assessments can be reused, so nobody has to start from scratch.
    </p>
    <!-- TODO Laís: add the slides link if you want to share them
    <p><a href="#">Slides (PDF)</a></p>
    -->
  </div>

  <figure class="figure">
    <img src="{{ '/assets/images/eeicat-figure.jpg' | relative_url }}"
         alt="Four-panel illustration of a freshwater ecosystem. A: native fish assemblage before the introduction of an alien fish. B: the alien fish affecting native population size, species loss, assemblage structure, growth, nutrients, soil and sediment, primary production and ecological function. C: impact magnitudes classified with EICAT, where several impacts cannot be assessed. D: the same impacts classified with EEICAT, each receiving a severity category."
         width="1808" height="1848" loading="lazy">
    <figcaption>
      Impacts of an alien species on a freshwater ecosystem classified with EICAT
      and EEICAT. (A) Ecosystem without the alien species. (B) Ecosystem impacted
      by the alien species; numbers indicate impact mechanisms. (C) Impact
      magnitudes under EICAT, where impacts beyond native populations cannot be
      classified (X). (D) Impact magnitudes under EEICAT. MC, Minimal Concern;
      MN, Minor; MO, Moderate; MR, Major.
      <span class="figure__credit">
        Reproduced from Carneiro et al. (2026),
        <a href="https://doi.org/10.1371/journal.pbio.3003665" target="_blank" rel="noopener"><i>PLOS Biology</i> 24(3), e3003665</a>,
        under a <a href="https://creativecommons.org/licenses/by/4.0/" target="_blank" rel="noopener">CC BY 4.0</a> licence.
      </span>
    </figcaption>
  </figure>
</section>

<section class="shell section">
  <h2>Key terms</h2>
  <dl class="terms">
    <div>
      <dt>Non-native (alien) species</dt>
      <dd>A species introduced by human activities outside its natural range.</dd>
    </div>
    <div>
      <dt>Invasive non-native species</dt>
      <dd>A population of an established non-native species that is spreading within its introduced range (Soto et al. 2024).</dd>
    </div>
    <div>
      <dt>Impact mechanism</dt>
      <dd>The process through which a non-native species causes an impact, such as predation, competition, hybridisation or disease transmission. EICAT recognises 12 mechanisms.</dd>
    </div>
    <div>
      <dt>Impact type</dt>
      <dd>The ecological change resulting from a mechanism, such as a population decline, a shift in community composition or an alteration of nutrient cycling. Carneiro et al. (2025) identify 19 impact types.</dd>
    </div>
    <div>
      <dt>Invasion event</dt>
      <dd>A non-native population in a given invaded area. It is the unit of assessment in EEICAT, whereas EICAT assesses the species as a whole.</dd>
    </div>
    <div>
      <dt>Severity categories</dt>
      <dd>Minimal Concern (MC), Minor (MN), Moderate (MO), Major (MR) and Massive (MV), shared by EICAT and EEICAT.</dd>
    </div>
  </dl>
</section>

<section class="shell section">
  <h2>References and further reading</h2>
  <nav aria-label="Reference sections">
    <ol class="toc">
      {% for s in sections %}
        <li><a href="#{{ s.id }}">{{ s.title }}</a></li>
      {% endfor %}
    </ol>
  </nav>

  {% for s in sections %}
    <div class="year-group" id="{{ s.id }}">
      <h2 class="year-group__heading">{{ s.title }}</h2>
      {% if s.intro %}<p class="group-intro">{{ s.intro }}</p>{% endif %}
      {% for item in s.items %}
        {% include publication.html pub=item %}
      {% endfor %}
    </div>
  {% endfor %}
</section>

<section class="shell section">
  <div class="section__lead">
    <h2>Contact</h2>
    <p>
      Questions and comments on EEICAT are welcome. Professional profiles are
      linked on the <a href="{{ '/' | relative_url }}">home page</a>, and the full
      list of publications is available on the
      <a href="{{ '/publications.html' | relative_url }}">publications page</a>.
    </p>
  </div>
</section>
