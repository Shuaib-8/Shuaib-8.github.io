---
permalink: /sitemap.xml
---
<?xml version="1.0" encoding="UTF-8" ?>
<urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">
{% for post in site.posts %}
{% include sitemap-entry.xml entry=post %}
{% endfor %}

{% for pages in site.pages %}
{% if page.layout %}
  {% include sitemap-entry.xml entry=pages %}
{% endif %}
{% endfor %}
</urlset>
