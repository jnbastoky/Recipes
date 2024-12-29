<ul>
  {% for page in site.static_files %}
    {% if page.name != 'index.md' and page.name != 'README.md' %}
      <li><a href="{{ page.path | remove_first: '/' }}">{{ page.basename }}</a></li>
    {% endif %}
  {% endfor %}
</ul>

<pre>
{{ site | inspect }}
</pre>
