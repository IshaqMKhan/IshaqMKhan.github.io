---
layout: archive
title: "Sitemap"
permalink: /sitemap/
author_profile: true
---

{% include base_path %}

A list of all the posts and pages found on the site.

<h2>Selected Pages</h2>

{% assign wanted_pages = "/publications/,/presentations/,/cv/" | split: "," %}

{% for page in site.pages %}
  {% assign page_url = page.url | append: "/" %}
  {% if wanted_pages contains page_url %}
    <h3><a href="{{ page.url }}">{{ page.title }}</a></h3>
    <div>{{ page.content }}</div>
  {% endif %}
{% endfor %}

<h2>Posts</h2>

{% for post in site.posts %}
  {% include archive-single.html %}
{% endfor %}

{% capture written_label %}'None'{% endcapture %}

{% for collection in site.collections %}
  {% unless collection.output == false or collection.label == "posts" %}
    {% capture label %}{{ collection.label }}{% endcapture %}
    {% if label != written_label %}
      <h2>{{ label | capitalize }}</h2>
      {% capture written_label %}{{ label }}{% endcapture %}
    {% endif %}
    {% for doc in collection.docs %}
      {% unless collection.output == false or collection.label == "posts" %}
        {% include archive-single.html %}
      {% endunless %}
    {% endfor %}
  {% endunless %}
{% endfor %}
