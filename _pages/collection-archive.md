---
layout: archive
title: "Assets"
permalink: /collection-archive/
author_profile: true
#entries_layout: grid
header:
  overlay_image: /assets/images/home/oddworld_header.jpg
  caption: "Photo credit: [**Oddworld inhabitants**](http://www.oddworld.com/)"
---
[Materials](#materials){: .btn .btn--light-outline .btn--small} [All assets](#all-assets){: .btn .btn--light-outline .btn--small}
{: style="text-align: center;"}

---

#### Materials 2019
{% capture written_label %}'None'{% endcapture %}

{% for collection in site.collections %}
  {% for post in collection.docs %}
    {% unless collection.output == false or collection.label != "materials" %}
      {% include archive-single.html type=page.entries_layout %}
    {% endunless %}
  {% endfor %}
{% endfor %}
<font size=”1”> [Back to Top ↑](#) </font>
{: style="text-align: right;"}

---

#### All assets
{% capture written_label %}'None'{% endcapture %}

{% for collection in site.collections %}
  {% for post in collection.docs %}
    {% unless collection.output == false or collection.label == "posts" %}
      {% include archive-single.html type=page.entries_layout %}
    {% endunless %}
  {% endfor %}
{% endfor %}
---
