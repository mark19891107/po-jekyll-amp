---
layout: default
permalink: /open-gov
---

{% for section in site.data.og.sections %}
{% assign loopindex = forloop.index | modulo: 2 %}
{% include section.html section=section index=loopindex %}
{% endfor %}
