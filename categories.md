---
layout: default
title: products
---
## All Products

<table>
	<tr>
		<th>ID</th>
		<th>Name</th>
		<th>Description</th>
		<th>Products</th>
	</tr>
	{% for k in site.data.categories %}
	<tr>
		<td>{{k.CategoryID}}</td>
		<td>{{k.CategoryName}}</td>
		<td>{{k.Description}}</td>
		<td>
			<ul>
			{% for p in k.products %}
				<li><a href="/products/{{p.ProductID}}.html">{{p.ProductName}}</a></li>
			{% endfor %}
			</ul>
		</td>
	</tr>
	{% endfor %}
</table>