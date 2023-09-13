---
layout: home
title: Home
permalink: /:path/
nav_order: 1
seo:
  type: Course
  name: Home
---

# toki!

Welcome to the Conlang DeCal, run by the [Society of Linguistics Undergraduate Students (SLUgS)](http://slugs.berkeley.edu/)!

We will meet on Tuesdays at 5-6:30pm in [Etcheverry 3107](https://goo.gl/maps/fFyejvbF3BQ6mfXp9). 
<br>
We will also hold hybrid office hours on Wednesdays at 3-4pm. You may attend in-person in [the Linguistics Lounge (Dwinelle 1203)](https://goo.gl/maps/ijwJZkd7UjrLRtNU7), or remotely through the class Discord server.
## Calendar
{% for module in site.modules %}
{{ module }}
{% endfor %}
## Staff
Our faculty advisor is [Prof. Peter Jenks](https://linguistics.berkeley.edu/~jenks/).
{% assign instructors = site.staffers | where: 'role', 'Instructor' %}
{% for staffer in instructors %}
{{ staffer }}
{% endfor %}
