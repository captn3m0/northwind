---
layout: default
title: products
---
## All Products

<table>
	<tr>
		<th>ID</th>
		<th>Name</th>
		<th>Stock Status</th>
	</tr>
	{% for k in site.data.products %}
	<tr>
		<td>{{k.ProductID}}</td>
		<td><a href="/products/{{k.ProductID}}.html">{{k.ProductName}}</a></td>
		<td>{{k.UnitsInStock}}</td>
	</tr>
	{% endfor %}
</table>