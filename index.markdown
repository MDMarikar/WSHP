---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: default
---

{% include google-search.html %}


{% assign sorted_items = site.my_collection | sort:"title" %}
{% for item in sorted_items %}
- [{{ item.title }}]({{ site.baseurl }}{{ item.url }})
{% endfor %}
