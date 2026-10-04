---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% include base_path %}

<ul class="pub-list">
{% for post in site.publications reversed %}
  {% if post.venue == 'The Extractive Industries and Society' %}
  </ul>
  <div style="display: flex; align-items: center; margin: 1.5em 0 1em 0;">
    <hr style="flex: 1; border: none; border-top: 1px solid #999;">
    <span style="padding: 0 0.8em; font-size: 0.85em; color: #666; white-space: nowrap;">pre-doctoral work</span>
    <hr style="flex: 1; border: none; border-top: 1px solid #999;">
  </div>
  <ul class="pub-list">
  {% endif %}
  <li>
    {% if post.paperurl %}<a href="{{ post.paperurl }}">{{ post.title }}</a>{% else %}{{ post.title }}{% endif %}<br>
    {% if post.coauthors %}({{ post.coauthors }})<br>{% endif %}
    {% if post.journal_cite %}{{ post.journal_cite }}{% endif %}
    {% if post.pdfurl or post.wpurl %}<br><span class="pub-links">{% if post.pdfurl %}<a href="{{ post.pdfurl }}">[published version]</a>{% endif %}{% if post.wpurl %} <a href="{{ post.wpurl }}">[working paper]</a>{% endif %}{% if post.slidesurl %} <a href="{{ post.slidesurl }}">[slides]</a>{% endif %}{% if post.posterurl %} <a href="{{ post.posterurl }}">[poster]</a>{% endif %}{% if post.oneearthurl %} <a href="{{ post.oneearthurl }}">[commentary]</a>{% endif %}{% if post.fundingurl %} <a href="{{ post.fundingurl }}">[funding]</a>{% endif %}{% if post.presentationurl %} <a href="{{ post.presentationurl }}">[presentation]</a>{% endif %}</span>{% endif %}
  </li>
{% endfor %}
</ul>
