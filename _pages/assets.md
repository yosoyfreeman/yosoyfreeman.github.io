---
title: Assets
layout: collection
layout: archive
title: "Assets"
permalink: /assets/
author_profile: true
#entries_layout: grid
header:
  overlay_image: /assets/images/home/oddworld_header.jpg
  caption: "Photo credit: [**Oddworld inhabitants**](http://www.oddworld.com/)"
---
[Materials](#materials){: .btn .btn--light-outline .btn--small} [All assets](#all-assets){: .btn .btn--light-outline .btn--small}
---
{: style="text-align: center;"}
---

### Materials
{% capture written_label %}'None'{% endcapture %}

{% for collection in site.collections %}
  {% for post in collection.docs %}
    {% unless collection.output == false or collection.label != "materials" %}
      {% include archive-single.html type=page.entries_layout %}
    {% endunless %}
  {% endfor %}
{% endfor %}
<p align="right">
        <font size="2"> <a href="#page-title">BACK TO TOP ↑</a> </font>  
</p>

---

### All assets
{% capture written_label %}'None'{% endcapture %}

{% for collection in site.collections %}
  {% for post in collection.docs %}
    {% unless collection.output == false or collection.label == "posts" %}
      {% include archive-single.html type=page.entries_layout %}
    {% endunless %}
  {% endfor %}
{% endfor %}
<p align="right">
        <font size="2"> <a href="#page-title">BACK TO TOP ↑</a> </font>  
</p>

---
      {% include archive-single.html type=page.entries_layout %}
    {% endunless %}
  {% endfor %}
{% endfor %}
