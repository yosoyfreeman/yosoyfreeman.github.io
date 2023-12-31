---
layout: archive
title: "Assets"
permalink: /collection-archive/
author_profile: true
header:
  overlay_image: /assets/images/home/oddworld_header.jpg
  actions:
  caption: "Photo credit: [**Oddworld inhabitants**](http://www.oddworld.com/)"
---

## Materials

---
{% capture written_label %}'None'{% endcapture %}

{% for collection in site.collections %}
  {% for post in collection.docs %}
    {% unless collection.output == false or collection.label != "materials" %}
      {% include archive-single.html type=page.entries_layout %}
    {% endunless %}
  {% endfor %}
{% endfor %}
