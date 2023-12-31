---
layout: single
title: "Assets"
permalink: /collection-archive/
author_profile: true
#entries_layout: grid
header:
  overlay_image: /assets/images/home/oddworld_header.jpg
  caption: "Photo credit: [**Oddworld inhabitants**](http://www.oddworld.com/)"
---
[Materials](#Materials){: .btn .btn--light-outline} [Sort by category](#){: .btn .btn--light-outline} [Sort by tag](/tags){: .btn .btn--light-outline}
---
## Materials
{% capture written_label %}'None'{% endcapture %}

{% for collection in site.collections %}
  {% for post in collection.docs %}
    {% unless collection.output == false or collection.label != "materials" %}
      {% include archive-single.html type=page.entries_layout %}
    {% endunless %}
  {% endfor %}
{% endfor %}

## more Materials
