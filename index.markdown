---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: My Collection
---

# My Collection

{% for item in site.my_collection %}
- [{{ item.title }}]({{ site.baseurl }}{{ item.url }})
{% endfor %}
