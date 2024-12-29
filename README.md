# Recipes
Personal Recipes

Edits made with https://www.noteshub.app/

<ul>
  {% for page in site.pages %}
    {% if page.path contains '.html' and page.path != 'index.html' and page.path != 'toc.html' %} {# Only list HTML files, excluding index and toc #}
      <li><a href="{{ page.url }}">{{ page.title | default: page.name | remove: '.html' | replace: '-', ' ' | capitalize }}</a></li>
    {% endif %}
  {% endfor %}
</ul>
