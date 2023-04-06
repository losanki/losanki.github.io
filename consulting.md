---
layout: page
title: Consulting
permalink: /consulting/
---
I am available for work related to IT such as design, development and implementation.
There are three modes available for contract work:
* Per hour
* Based on service
* Long term contract

### Per hour flat charges:
Available for hourly charges of rs 1000 or $15.

### Per service:  

<table>
<th>Service</th><th>Details</th><th>Cost</th>
{% for row in site.services %}
<tr><td><a href="{{row.url}}">{{ row.title }}</a></td><td>{{ row.description }}</td><td>{{ row.cost }}</td></tr>

{% endfor %}
</table>

### Long term contract:
Awailable for remote work and office visits in case the client is in Bengaluru area for 
upto twice a week. Please contact me for charges.

### Development:  
Experience with Django, flask, Python, Vuejs, html, css, javascript  


