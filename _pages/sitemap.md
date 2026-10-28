---
layout: archive
title: "Sitemap"
permalink: /sitemap/
author_profile: true
---

{% include base_path %}

<div class="page__content">

<h2>Pages</h2>
<ul>
  <li><a href="{{ base_path }}/">About</a></li>
  <li><a href="{{ base_path }}/portfolio/">Research</a></li>
  <li><a href="{{ base_path }}/publications/">Publications</a></li>
  <li><a href="{{ base_path }}/cv/">CV</a></li>
</ul>

<h2>Research projects</h2>
<ul>
{% assign projects = site.portfolio | sort: "order" %}
{% for p in projects %}
  <li><a href="{{ base_path }}{{ p.url }}">{{ p.title }}</a></li>
{% endfor %}
</ul>

<p>An <a href="{{ base_path }}/sitemap.xml">XML version</a> is also available.</p>

</div>
