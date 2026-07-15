---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% include base_path %}

<ul class="pub-list">
{% for post in site.publications reversed %}
  <li>
    {% if post.paperurl %}<a href="{{ post.paperurl }}">{{ post.title }}</a>{% else %}{{ post.title }}{% endif %}<br>
    {% if post.coauthors %}({{ post.coauthors }})<br>{% endif %}
    {% if post.journal_cite %}{{ post.journal_cite }}{% endif %}
    {% if post.wpurl %}<br><span class="pub-links">{% if post.pdfurl %}<a href="{{ post.pdfurl }}">[published version]</a>{% else %}<a href="{{ post.paperurl }}">[published version]</a>{% endif %} <a href="{{ post.wpurl }}">[working paper]</a>{% if post.posterurl %} <a href="{{ post.posterurl }}">[poster]</a>{% endif %}{% if post.oneearthurl %} <a href="{{ post.oneearthurl }}">[One Earth article]</a>{% endif %}</span>{% endif %}
  </li>
{% endfor %}
</ul>
