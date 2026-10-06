---
title: 'Others'
date: 2026-10-05 00:00:00
description: Others
featured_image: '/images/others/others.jpg'
---

<div class="gallery" data-columns="3">
	{% assign image_files = site.static_files | where: "others", true | sort: 'basename' | reverse %}
	{% for image in image_files %}
		<img src="{{ image.path }}">
	{% endfor %}
</div>
