---
title: "Photos that I enjoy"
permalink: /photos/
author-profile: true
images:
  - image_path: http://mogryzko.github.io/images/DSC_1286.jpg
  - image_path: http://mogryzko.github.io/images/IMG_20171230_150856229_HDR.jpg
---

<ul class="photo-gallery">
  {% for image in page.images %}
    <li><img src="{{ image.image_path }}" alt="drawing" height = "400"/></li>
  {% endfor %}
</ul>





