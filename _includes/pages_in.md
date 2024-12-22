{% for page in site.pages %}
  {% if page.url contains include.folder %}
* [{% if page.title %}{{page.title}}{% else %}{{page.url}}{% endif %}]({{page.url}})
  {% endif %}
{% endfor %}
