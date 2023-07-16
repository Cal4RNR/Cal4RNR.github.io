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

- [View our Course Calendar](calendar.md), this is also where you will download starter files for our activities.
- [Meet our Staff](staff.md),
- View our [Schedule](schedule.md) on a traditional calendar format.

# Announcements

{% assign announcements = site.announcements | reverse %}
{% for announcement in announcements %}
{{ announcement }}
{% endfor %}
