---
title: 'Butterflies'
date: 2026-10-05 00:00:00
description: Enameled Butterflies
featured_image: '/images/butterflies/butterflies.jpg'
---

<div class="gallery" data-columns="3">
	{% assign image_files = site.static_files | where: "butterflies", true | sort: 'basename' | reverse %}
	{% for image in image_files %}
		<img src="{{ image.path }}">
	{% endfor %}
</div>
