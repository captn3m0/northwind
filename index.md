---
layout: default
title: northwind
---
# NORTHWIND

{% assign FP = site.data.featured.product[0] %}

## Have you tried our <a href="/products/{{FP.ProductID}}.html">{{FP.ProductName}}</a> yet? It is selling at {{FP.UnitPrice}}, go buy today.

{% assign employeeOfTheMonth = site.data.employeeOfTheMonth.first %}
## Congratulations {{employeeOfTheMonth.FirstName}} {{employeeOfTheMonth.LastName}} for being ⭐ employee of the month
