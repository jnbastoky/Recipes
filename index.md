<ul>
  {% for page in site.static_files %}
    {% if page.extname == '.md' and page.name != 'index.md' and page.name != 'README.md' %}
      <li><a href="{{ page.path | remove_first: '/' | replace: '.md', '' }}">{{ page.basename }}</a></li>
    {% endif %}
  {% endfor %}
</ul>

_Source on [GitHub][github-source]_

{% comment %}
<pre>
  {{ site | inspect }}
</pre>
{% endcomment %}

[github-source]: https://github.com/jnbastoky/Recipes
