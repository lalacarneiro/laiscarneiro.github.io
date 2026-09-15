---
layout: default
title: "Publications"
heading: "Publications"
subheading: "Peer-reviewed articles, newest first. A plum rule marks first-author papers."
description: "Peer-reviewed publications by Laís Carneiro on biological invasions and their ecological impacts."
permalink: /publications.html
---

<section class="shell section" style="border-top:0; padding-top:0">
  {% assign pubs = site.data.publications | sort: "year" | reverse %}
  {% assign years = pubs | map: "year" | uniq %}
  {% for year in years %}
    <div class="year-group">
      <h2 class="year-group__heading">{{ year }}</h2>
      {% for pub in pubs %}
        {% if pub.year == year %}
          {% include publication.html pub=pub %}
        {% endif %}
      {% endfor %}
    </div>
  {% endfor %}

  <p style="margin-top:2rem">
    The complete and always-current list lives on
    <a href="https://scholar.google.com/citations?user=rUvrtAsAAAAJ" target="_blank" rel="noopener">Google Scholar</a>
    and <a href="https://orcid.org/0000-0002-3828-7751" target="_blank" rel="noopener">ORCID</a>.
  </p>
</section>
