---
layout: page
title: Puree.app Help
permalink: /
---

# Within [Puree](https://puree.app) we offer both the Help Center and tutorial videos.

We offer the following options to help answer your questions:
- A personal demo and walkthrough of Puree and its features (contact email@puree.app to book a time)
- Personal email support to our team at email@puree.app
- [Puree Helpsite](https://help.puree.app)

{% include callout.html text="We're here to help make Puree a success story for your business. Don't hesitate to get in touch if you have any questions." %}

{% assign toc = site.data.toc %} <!-- Load the toc.yml data -->
{% for section in toc %}
### {{ section.title }}
{% if section.links %}
  {% for link in section.links %}
- [{{ link.title }}]({{ link.url | prepend: site.baseurl }})
  {% endfor %}
{% endif %}
{% endfor %}
