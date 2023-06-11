---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: default
---


#previous unsorted list
#{% for item in site.my_collection %}
#- [{{ item.title }}]({{ site.baseurl }}{{ item.url }})
#{% endfor %}


code
{% assign sorted_items = site.my_collection | sort:"title" %}
{% for item in sorted_items %}
- [{{ item.title }}]({{ site.baseurl }}{{ item.url }})
{% endfor %}
