# Recipes
Personal Recipes

Edits made with https://www.noteshub.app/

<ul>
  {% for file in site.static_files %}
    <li><a href="{{ file.path }}">{{ file.path }}</a></li>
  {% endfor %}
</ul>
