---
layout: home
title: Just the Class
nav_exclude: true
permalink: /:path/
seo:
  type: Course
  name: Just the Class
---

# Peer Rising Summer 2023

Welcome! This is the landing page for our official website for the course. You will find all important information on the left navigation bar, or click the links below. Our announcements will also be posted on this page, updated daily.

- [Course Calendar](calendar.md),
- [Staff](staff.md) page,
- [schedule](schedule.md).

# Announcements

Announcements are stored in the `_announcements` directory and rendered according to the layout file, `_layouts/announcement.html`.

{% assign announcements = site.announcements | reverse %}
{% for announcement in announcements %}
{{ announcement }}
{% endfor %}
