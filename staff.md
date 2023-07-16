---
layout: page
title: Staff
description: A listing of all the course staff members.
---

# Staff

Say hello to our staff!

## Instructors

{% assign instructors = site.staffers | where: 'role', 'Instructor' %}
{% for staffer in instructors %}
{{ staffer }}
{% endfor %}

{% assign advisors = site.staffers | where: 'role', 'Advisor' %}
{% assign num_advisors = advisors | size %}
{% if num_advisors != 0 %}
## Teaching Assistants

{% for staffer in advisors %}
{{ staffer }}
{% endfor %}
{% endif %}

{% assign pets = site.staffers | where: 'role', 'Pets' %}
{% assign num_pets = pets | size %}
{% if num_pets != 0 %}
## Teaching Assistants

{% for staffer in pets %}
{{ staffer }}
{% endfor %}
{% endif %}

