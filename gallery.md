---
layout: gallery
title: Photo Gallery
permalink: /gallery/
---
{% for image in site.data.gallery %}
  ![{{image.alt}}](/assets/images/{{ image.file }}.jpg)
{% endfor %}