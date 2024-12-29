<ul>
  {% for page in static_files %}
    <li><a href="{{ page.path | slice: 1 }}">{{ page.basename }}</a></li>
  {% endfor %}
</ul>
{% for page in static_files %}
  <a href="{{ page.path | slice: 1 }}">{{ page.basename }}</a><br>
{% endfor %}
