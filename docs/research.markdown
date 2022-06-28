---
layout: page
title: Research
permalink: /research

pubs: 
  - title:   "Ferrers Graphs, D-Permutations, and Surjective Staircases"
    author:  "A. Lazar"
    journal: "The Ramanujan Journal"
    year:    "2022"
    url:     "https://link.springer.com/article/10.1007/s11139-022-00581-5"
    
  - title:   "The Homogenized Linial Arrangement and Genocchi Numbers"
    author:  "A. Lazar, M. Wachs"
    journal: "Combinatorial Theory"
    year:    "2022"
    url:     "https://doi.org/10.5070/C62156874"    
---

My research is in algebraic, enumerative, and topological combinatorics. I'm particularly interested in problems involving hyperplane arrangements, 
Young tableaux, and permutation enumeration, as well as in structural questions about the topology of simplicial complexes.

## Published Papers

{% for pub in page.pubs %}
[**{{pub.title}}**]({% if pub.internal %}{{pub.url | prepend: site.baseurl}}{% else %}{{pub.url}}{% endif %})<br />
{{pub.author}}<br />
*{{pub.journal}}*
{% if pub.note %} *({{pub.note}})*
{% endif %} *{{pub.year}}* {% if pub.doi %}[[doi]({{pub.doi}})]{% endif %}
{% endfor %}
