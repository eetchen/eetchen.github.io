---
layout: archive
title: 'Publications'
permalink: publications/
entries_layout: grid
type: grid
author_profile: true
---

{% if author.googlescholar %}
You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

<!-- <h2>Journal Articles</h2> -->

<h2 style="margin: 0px 0px 20px; font-weight: normal; line-height: 1.5em; font-family: Georgia">Journal Articles:</h2>

{% for post in site.publications reversed %}
{% if post.pubtype == 'journal' %}
{% include archive-single.html%}
{% endif %}
{% endfor %}

<!-- <h2>Conference Papers</h2> -->
<h2 style="margin: 0px 0px 20px; font-weight: normal; line-height: 1.5em; font-family: Georgia;">Conference Papers:</h2>
{% for post in site.publications reversed %}
{% if post.pubtype == 'conference' %}
{% include archive-single.html %}
{% endif %}
{% endfor %}
