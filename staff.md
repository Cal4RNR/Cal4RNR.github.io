---
layout: page
title: Staff
description: A listing of all the course staff members.
---

# Staff

Staff information is stored in the `_staffers` directory and rendered according to the layout file, `_layouts/staffer.html`.

## Instructors

{% assign instructors = site.staffers | where: 'role', 'Instructor' %}
{% for staffer in instructors %}
{{ staffer }}
{% endfor %}

{% assign advisors = site.staffers | where: 'role', 'Advisors' %}
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

