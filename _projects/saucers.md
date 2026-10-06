---
title: 'Saucers'
date: 2026-10-05 00:00:00
description: Cloissone Saucers
featured_image: '/images/saucers/saucers.jpg'
---

<div class="gallery" data-columns="3">
	{% assign image_files = site.static_files | where: "saucers", true | sort: 'basename' | reverse %}
	{% for image in image_files %}
		<img src="{{ image.path }}">
	{% endfor %}
</div>
