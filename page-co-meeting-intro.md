---
layout: default
permalink: /collaborative-meeting
---

{% for flow in site.data.co-meeting.flows %}
{% assign loopindex = forloop.index | modulo: 2 %}
{% include flow.html flow=flow index=loopindex %}
{% endfor %}
