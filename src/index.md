---
layout: layout.html
pageTitle: New York Today
pageClass: home
navTitle: Home
tags: page
---

## Articles

<button>Show Stories</button>

<main class="stories"></main>

{% for page in collections.page %}

<h2><a href="{{ page.url }}">{{ page.data.pageTitle | upcase }}</a></h2>
<em>{{ page.date | date: "%Y-%m-%d" }}</em>
{% endfor %}
