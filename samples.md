---
title: Samples
permalink: /samples
layout: default
---
# Sample Code and Exercises

<div class="samples">
	<ul class="post-list">
		{% assign samples = site.samples | where: "hidden", "false" %}
		{% for sample in samples %}
            <li>
                <h2><a class="post-link" href="{{ sample.url | relative_url }}">{{ sample.title | escape }}</a></h2>
                <span class="post-meta">{{ sample.excerpt }}</span>
            </li>
		{% endfor %}
	</ul>
</div>
