---
layout: default
---

<h1>{{page.product.ProductName}}</h1>

<table>
	{% for k in page.product %}
	<tr>
		<th>{{k[0]}}</th>
		<td>{{k[1]}}</td>
	</tr>
	{% endfor %}
</table>