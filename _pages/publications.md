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
  </li>
{% endfor %}
</ul>
