---
title: Resources
child_type: resource
published: true
content:
    items: '@self.children'
    order:
        by: date
        dir: desc
    limit: 10
    pagination: true
---

{% for p in page.collection %}
<h2>{{ p.title|e }}</h2>
{{ p.summary|raw }}
{% endfor %}