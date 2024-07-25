---
layout: default
---

<h1>{{page.customer.CompanyName}}</h1>

<table>
	{% for k in page.customer %}
	<tr>
		<th>{{k[0]}}</th>
		<td>{{k[1]}}</td>
	</tr>
	{% endfor %}
</table>