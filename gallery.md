---
layout: gallery
title: Gallery
permalink: /gallery/
---
{% assign gallery_images = site.static_files | where: "gallery_image", true %}
{% for gallery_image in gallery_images %}
  ![{{ gallery_image.basename }}]({{ gallery_image.path }})
{% endfor %}