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
    <li><img src="{{ image.image_path }}" alt="drawing" width = "200"/></li>
  {% endfor %}
</ul>

<p id="test"></p>
<div class = "fullwidth">
  <div id="chart"></div>
</div>
<div id="viewof-slider"></div>
<div id="viewof-gender"></div>
<div id="viewof-type"></div>

<script type="module">
  import notebook from "https://api.observablehq.com/@mogryzko/assignment-3/2.js";

  const renders = {
    "test": "#test",
    "chart": "#chart",
    "viewof slider": "#viewof-slider",
    "viewof gender": "#viewof-gender",
    "viewof type": "#viewof-type",
  };

  import {Inspector, Runtime} from "https://unpkg.com/@observablehq/notebook-runtime@1.2.0?module";
  for (let i in renders)
    renders[i] = document.querySelector(renders[i]);

  Runtime.load(notebook, (variable) => {
    if (renders[variable.name])
      return new Inspector(renders[variable.name]);
  });
</script>





