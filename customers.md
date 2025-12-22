---
layout: default
title: customers
---
## All Customers

<table>
	<tr>
		<th>ID</th>
		<th>Company Name</th>
		<th>Contact Name</th>
		<th>Title</th>
		<th>Address</th>
	</tr>
	{% for k in site.data.customers %}
	<tr>
		<td>{{k.CustomerID}}</td>
		<td><a href="/customers/{{k.Country}}/{{k.CustomerID}}/">{{k.CompanyName}}</a></td>
		<td>{{k.ContactName}}</td>
		<td>{{k.ContactTitle}}</td>
		<td>{{k.City}}, {{k.Country}}</td>
	</tr>
	{% endfor %}
</table>