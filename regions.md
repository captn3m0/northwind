---
layout: default
title: Region-Wise Employees
---
# Region-wise Employees

{% for R in site.data.regions %}
# {{R.RegionDescription}}

{% for T in R.territories %}
## {{T.TerritoryDescription}}
<ul>
{% for E in T.employees %}
<li>{{E.LastName}}, {{E.FirstName}}</li>
{% endfor %}
</ul>
{% endfor %}
{% endfor %}