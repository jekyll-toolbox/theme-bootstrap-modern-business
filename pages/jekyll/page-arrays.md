---
layout: jekyll-demo
title: Jekyll Demo | Page Arrays

data: [ Eins: { 'Eins', 1 }, Zwei: { 'Zwei', 1 } ]
---
<di>
<h1>Demo Page: Accessing arrays<h1>
{% include page-arrays.html %}

<h1>Demo: Accessing collections<h1>
<b>for team: start</b>

{% for team in site.teams %}
    <li>team = {{ team }}. name={{ team.name }} </li>
{% endfor %}
<b>for team: done</b>
