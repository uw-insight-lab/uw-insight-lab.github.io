---
permalink: /publications/
layout: home
author_profile: true
title: "Publications"
---

{% assign publications = site.data.publications %}

{% assign years = publications | map: "year" | uniq | sort | reverse %}

{% for year in years %}
  {% assign pubs_for_year = publications | where: "year", year %}
  {% include pubs-list.html arr=pubs_for_year yr = year %}
{% endfor %}

