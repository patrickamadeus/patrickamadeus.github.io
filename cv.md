---
layout: homepage
permalink: /cv/
title_prefix: CV
---
{% assign cv = site.data.cv %}
<a class="back-link" href="{{ '/' | relative_url }}">&larr; {{ site.title }}</a>

<div class="cv">
<div class="cv-head">
  <h1>{{ cv.name }}</h1>
  <p class="cv-contacts">{% for c in cv.contacts %}{% unless forloop.first %} &middot; {% endunless %}{% if c.url %}<a href="{{ c.url }}">{{ c.label }}</a>{% else %}{{ c.label }}{% endif %}{% endfor %}</p>
  <p><a class="cv-download" href="{{ site.cv_link | relative_url }}?v={{ site.time | date: '%Y%m%d%H%M' }}" target="_blank" rel="noopener">View PDF &#8599;</a></p>
</div>

<h2>Research Interests</h2>
<p>{% assign parts = cv.summary | split: "**" %}{% for part in parts %}{% assign r = forloop.index0 | modulo: 2 %}{% if r == 1 %}<strong>{{ part }}</strong>{% else %}{{ part }}{% endif %}{% endfor %}</p>
<p><strong>Research Areas:</strong> <em>{{ cv.interests | join: ", " }}</em></p>

<h2>Education</h2>
{% for e in cv.education %}
<div class="cv-row"><span><strong>{{ e.degree }} — {{ e.school }}</strong></span><span class="cv-date">{{ e.date }}</span></div>
<p class="cv-sub">{% if e.detail_url %}{% assign link_html = '<a href="' | append: e.detail_url | append: '">' | append: e.detail_link | append: '</a>' %}{{ e.detail | replace: e.detail_link, link_html }}{% else %}{{ e.detail }}{% endif %}</p>
{% endfor %}

<h2>Publications <span class="h2-aside">({{ cv.publications_note }})</span></h2>
<ul class="pubs cv-pubs">
{% for p in cv.publications %}
<li>
  {% if p.url %}<a class="pub-title" href="{{ p.url }}" target="_blank" rel="noopener">{{ p.title }}</a>{% else %}<span class="pub-title nolink">{{ p.title }}</span>{% endif %}{% if p.marker %}<sup>{{ p.marker }}</sup>{% endif %}
  <div class="cv-row"><span class="cv-keywords">{{ p.keywords }}</span><span class="cv-date">{{ p.venue }}{% if p.award %} (<span class="pub-note">{{ p.award }}</span>){% endif %}</span></div>
</li>
{% endfor %}
</ul>

<h2>Work Experience</h2>
{% for x in cv.experience %}
<div class="cv-row"><span><strong>{{ x.role }}</strong>, {{ x.org }}</span><span class="cv-date">{{ x.date }}</span></div>
<ul class="cv-bullets">
{% for b in x.bullets %}<li>{{ b }}</li>{% endfor %}
</ul>
{% endfor %}

<h2>Achievement &amp; Awards</h2>
{% for h in cv.honors %}
<div class="cv-row"><span>{{ h.name }}</span><span class="cv-date">{{ h.date }}</span></div>
{% endfor %}

<h2>Advising &amp; Mentorship</h2>
{% for m in cv.mentorship %}
<div class="cv-row"><span><strong>{{ m.name }}</strong>, <em>{{ m.topic }}</em></span><span class="cv-date">{{ m.now }}</span></div>
{% endfor %}

<h2>References</h2>
{% for r in cv.references %}
<div class="cv-row"><span><strong>{{ r.name }}</strong>, {{ r.title }}</span><span class="cv-date"><a href="mailto:{{ r.email }}">{{ r.email }}</a></span></div>
{% endfor %}
</div>
