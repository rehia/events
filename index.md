---
layout: default
---

{% for event in site.posts %}
## {{ event.title }}
{{ event.date | date_to_long_string }}

{{ event.excerpt }}
[En savoir plus...]({{ site.baseurl }}{{ event.url }})
{% endfor %}
