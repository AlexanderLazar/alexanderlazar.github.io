---
layout: page
permalink: /research/
title: Research
pubs:
    - title:   "Ferrers Graphs, D-Permutations, and Surjective Staircases"
      author:  "A. Lazar"
      journal: "The Ramanujan Journal"
      year:    "2022"
      url:     "https://link.springer.com/article/10.1007/s11139-022-00581-5"
    
    - title:   "Partition and Cohen--Macaulay Extenders"
      author:  "J. Doolittle, B. Goeckner, A. Lazar"
      journal: "European Journal of Combinatorics"
      year:    "2022"
      url:     "https://www.sciencedirect.com/science/article/pii/S0195669821001827"
    
    - title:   "The Homogenized Linial Arrangement and Genocchi Numbers"
      author:  "A. Lazar, M. Wachs"
      journal: "Combinatorial Theory"
      year:    "2022"
      url:     "https://doi.org/10.5070/C62156874"
    
    - title:   "A Chip-Firing Game on the Product of Two Graphs and the Tropical Picard Group"
      author:  "A. Lazar"
      journal: "Electronic Journal of Combinatorics"
      year:    "2017"
      url:     "https://www.combinatorics.org/ojs/index.php/eljc/article/view/v24i4p14"


pres:
    - title:   "On the q-Enumeration of Barely Set-Valued Plane Partitions and Linear Extensions"
      author:  "S. Hopkins, A. Lazar, S. Linusson"
      #journal: "arXiv"
      year:    "2021"
      url:     "https://arxiv.org/abs/2106.07418"
    
abs:   
    - title:   "On the Homogenized Linial Arrangement: Intersection Lattice and Genocchi Numbers"
      author:  "A. Lazar, M. Wachs"
      journal: "S&eacute;minaire Lotharingien de Combinatoire"
      #note: "Extended Abstract"
      year:    "2019"
      url:     "https://www.mat.univie.ac.at/~slc/wpapers/FPSAC2019/93.html"
slides:
    - title: "Lexicographic Shellability Statistics"
      venue: "NORCOM 2022"
      location: "Troms&oslash;, Norway"
      url: "/slides/NORCOM.pdf"
---

My research is in algebraic, enumerative, and topological combinatorics. I'm particularly interested in problems involving hyperplane arrangements, 
Young tableaux, and permutation enumeration, as well as in structural questions about the topology of simplicial complexes.

## Published Papers

{% for pub in page.pubs %}
[**{{pub.title}}**]({% if pub.internal %}{{pub.url | prepend: site.baseurl}}{% else %}{{pub.url}}{% endif %})<br />
{{pub.author}}<br />
*{{pub.journal}}*
{% if pub.note %} *({{pub.note}})*
{% endif %} *({{pub.year}})* {% if pub.doi %}[[doi]({{pub.doi}})]{% endif %}
{% endfor %}

## Preprints

{% for pub in page.pres %}
[**{{pub.title}}**]({% if pub.internal %}{{pub.url | prepend: site.baseurl}}{% else %}{{pub.url}}{% endif %})<br />
{{pub.author}} <br />
{% if pub.note %} *({{pub.note}})*
{% endif %} *{{pub.year}}* {% if pub.doi %}[[doi]({{pub.doi}})]{% endif %}
{% endfor %}

## Extended Abstracts
{% for pub in page.abs %}
[**{{pub.title}}**]({% if pub.internal %}{{pub.url | prepend: site.baseurl}}{% else %}{{pub.url}}{% endif %})<br />
{{pub.author}}<br />
*{{pub.journal}}*
{% if pub.note %} *({{pub.note}})*
{% endif %} *({{pub.year}})* {% if pub.doi %}[[doi]({{pub.doi}})]{% endif %}
{% endfor %}

## Talks
{% for pub in page.slides %}
[**{{pub.title}}**]({% if pub.internal %}{{pub.url | prepend: site.baseurl}}{% else %}{{pub.url}}{% endif %})<br />
{{pub.venue}}<br />
{{pub.location}}
{% endfor %}