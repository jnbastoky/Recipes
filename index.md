<ul>
  {% for page in site.static_files %}
    {% if page.extname == '.md' and page.name != 'index.md' and page.name != 'README.md' %}
      <li><a href="{{ page.path | remove_first: '/' | remove_last: '.md' }}">{{ page.basename }}</a></li>
    {% endif %}
  {% endfor %}
</ul>

{% comment %}
<pre>
  {{ site | inspect }}
</pre>
{% endcomment %}
