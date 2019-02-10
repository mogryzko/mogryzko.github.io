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



<script type="module">
  // Load the Observable runtime and inspector.
  import {Runtime, Inspector} from "https://unpkg.com/@observablehq/notebook-runtime?module";

  // Your notebook, compiled as an ES module.
  import notebook from "https://api.observablehq.com/@mogryzko/assignment-3/2.js";

  // Load the notebook, observing its cells with a default Inspector
  // that simply renders the value of each cell into the provided DOM node.
  Runtime.load(notebook, Inspector.into(document.body));
</script>





