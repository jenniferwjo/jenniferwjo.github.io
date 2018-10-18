---
exclude: true
---

Everything I Learned!

{% assign sessions = site.connecttech2018  %}
<ol>
  {% for item in sessions %}
  	{% unless item.exclude %}
    	<li><a href="{{item.url}}">{{item.title}}</a></li>
    {% endunless %}
  {% endfor %}
</ol>