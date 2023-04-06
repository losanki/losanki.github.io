---
layout: page
title: Consulting
permalink: /consulting/
---
I am available for design, development and implementation.
There are three modes available for work:
* Per hour
* Based on service
* Consulting contract

### Per hour flat charges:
Available for hourly charges of INR 2500 or USD $30.

### Per service:  

<table>
<th>Service</th><th>Details</th><th>Cost</th>
{% for row in site.services %}
<tr><td><a href="{{row.url}}">{{ row.title }}</a></td><td>{{ row.description }}</td><td>{{ row.cost }}</td></tr>

{% endfor %}
</table>

### Consulting contract:
INR 20000 retainer + INR 1000 per hour for development work 

### Development:  
Experience with Django, flask, Python, Vuejs, html, css, javascript  


