<ul>
  {% for file in site.static_files %}
    {% if file.path contains '.md' and file.path != 'README.md' and file.path != 'toc.md' %}
      {% assign filename = file.path | remove: '.md' %}
      <li><a href="/{{ filename | replace: ' ', '-' | downcase }}/">{{ filename | replace: '-', ' ' | capitalize }}</a></li>
    {% endif %}
  {% endfor %}
</ul>
