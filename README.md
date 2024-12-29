# Recipes
Personal Recipes

Edits made with https://www.noteshub.app/

<ul>
  {% for page in site.pages %}
    {% if page.path.end_with?('.md') and page.path != 'index.md' and page.path != 'toc.md' %} 
    <li><a href="{{ page.url | replace: '.md', '' }}">{{ page.title | default: page.name | remove: '.html' | replace: '-', ' ' | capitalize }}</a></li>
    {% endif %}
  {% endfor %}
</ul>

# Repository Contents

<pre>{{ site.pages | inspect }}</pre>
