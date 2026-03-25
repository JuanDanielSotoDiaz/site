---
layout: archive
title: "Publications (mostly pre-doctoral work)"
permalink: /publications/
author_profile: true
---

{% include base_path %}

<ul class="pub-list">
{% for post in site.publications reversed %}
  <li>
    {% if post.paperurl %}
      <a href="{{ post.paperurl }}">{{ post.citation }}</a>
    {% else %}
      {{ post.citation }}
    {% endif %}
  </li>
{% endfor %}
</ul>
