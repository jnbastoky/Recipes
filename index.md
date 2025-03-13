This is collection of personal recipes.  Most of these are created by me or are an adaption of other recipes.  There are often a work in progress and are updated from time to time.

## Table of Contents
<ul>
  {% for page in site.static_files %}
    {% if page.extname == '.md' and page.name != 'index.md' and page.name != 'README.md' %}
      <li><a href="{{ page.path | remove_first: '/' | replace: '.md', '' }}">{{ page.basename }}</a></li>
    {% endif %}
  {% endfor %}
</ul>

_Source on [GitHub][github-source]_
_Edits made with [NotesHub][NotesHub-site]_
_Site generated with [Jekyl][Jekyl-site]_

{% comment %}
<pre>
  {{ site | inspect }}
</pre>
{% endcomment %}

[github-source]: https://github.com/jnbastoky/Recipes
[NotesHub-site]: https://www.noteshub.app/
[Jekyl-site]: https://jekyllrb.com/
