---
title: "A blog"
permalink: /blog/
author-profile: true
images:
  - image_path: http://mogryzko.github.io/images/DSC_1286.jpg
  - image_path: http://mogryzko.github.io/images/IMG_20171230_150856229_HDR.jpg
---

<link href="https://mogryzko.github.io/main.css" rel="stylesheet" />

<p> <strong> Currently under construction </strong> </p>


<ul class="photo-gallery">
  {% for image in page.images %}
    <li><img src="{{ image.image_path }}" alt="drawing" width = "200"/></li>
  {% endfor %}
</ul>






