---
layout: page
title: Teaching
---
<!--
###### Current Courses
{% for course in site.teaching reversed %}
{% if course.layout == 'course_info' %}
{% if course.quarter == site.quarter %}

<!--
* [{% include course_listing.md %}]({{ site.baseurl }}{{ course.url }})
{% endif %}
<!--
{% endif %}
{% endfor %} -->

###### I served as a teaching assistant for the following courses at UCLA:
{% for course in site.teaching reversed %}
{% if course.quarter != site.quarter %}
{% if course.layout == 'course_info' %}

* {% include course_listing.md %}

{% endif %}
{% endif %}
{% endfor %}
