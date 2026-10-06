---
title: 'Pierceworks'
date: 2026-10-05 00:00:00
description: Pierceworks
featured_image: '/images/piercings/pierecing.jpg'
---

<div class="gallery" data-columns="3">
	{% assign image_files = site.static_files | where: "piercings", true | sort: 'basename' | reverse %}
	{% for image in image_files %}
		<img src="{{ image.path }}">
	{% endfor %}
</div>
