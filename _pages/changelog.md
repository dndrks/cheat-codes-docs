---
layout: page
title: changelog
permalink: /changelog/
---
{% assign changelog_by_order = site.changelog | reverse %}
{% for log in changelog_by_order %}
<h3>{{ log.version }}</h3>
<hr>
{{ log.content }}
{% endfor %}
