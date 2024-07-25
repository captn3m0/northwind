---
layout: default
title: restock
sqlite:
- data: restock
  query: "SELECT * FROM Products WHERE (UnitsInStock - ReOrderLevel) <=20 ORDER BY  UnitsInStock ASC"
  file: "_db/northwind.db"
---

## All Products

<table>
	<tr>
		<th>Name</th>
		<th>Stock Status</th>
	</tr>
	{% for k in page.restock %}
	<tr>
		<td><a href="/products/{{k.ProductID}}">{{k.ProductName}}</a></td>
		<td>{{k.UnitsInStock}}</td>
	</tr>
	{% endfor %}
</table>