<div class="publications publications-page">
  <h1>Publications</h1>
  <p class="publications-intro">
    Efficient multimodal learning <span aria-hidden="true">&middot;</span>
    Self-improving systems <span aria-hidden="true">&middot;</span>
    Multilingual and multicultural evaluation <span aria-hidden="true">&middot;</span>
    Multimodal reasoning and robustness
  </p>

  {% assign year_groups = site.data.publications.main | group_by: "year" | sort: "name" | reverse %}
  {% for year_group in year_groups %}
  <div class="publication-year" id="year-{{ year_group.name }}">
    <h2>{{ year_group.name }}</h2>
    <ol class="bibliography">
      {% for link in year_group.items %}
      <li>
        <div class="pub-row">
          {% if link.image %}
          <div class="col-sm-3 abbr publication-image">
            {% if link.pdf %}<a href="{{ link.pdf }}" target="_blank" rel="noopener">{% endif %}
            <img src="{{ link.image | relative_url }}" alt="Figure from {{ link.title }}" class="teaser img-fluid z-depth-1">
            {% if link.pdf %}</a>{% endif %}
            {% if link.conference_short %}
            <abbr class="badge">{{ link.conference_short }}</abbr>
            {% endif %}
          </div>
          {% endif %}
          <div class="publication-details">
            <div class="title">
              {% if link.pdf %}
              <a href="{{ link.pdf }}" target="_blank" rel="noopener">{{ link.title }}</a>
              {% elsif link.page %}
              <a href="{{ link.page }}" target="_blank" rel="noopener">{{ link.title }}</a>
              {% else %}
              {{ link.title }}
              {% endif %}
            </div>
            <div class="author">{{ link.authors }}</div>
            <div class="periodical"><em>{{ link.conference }}</em></div>
            {% if link.summary %}<div class="summary">{{ link.summary }}</div>{% endif %}
            <div class="links">
              {% if link.pdf %}<a href="{{ link.pdf }}" class="btn btn-sm z-depth-0" role="button" target="_blank" rel="noopener">PDF</a>{% endif %}
              {% if link.code %}<a href="{{ link.code }}" class="btn btn-sm z-depth-0" role="button" target="_blank" rel="noopener">Code</a>{% endif %}
              {% if link.page %}<a href="{{ link.page }}" class="btn btn-sm z-depth-0" role="button" target="_blank" rel="noopener">Project Page</a>{% endif %}
              {% if link.notes %}<strong class="publication-note">{{ link.notes }}</strong>{% endif %}
            </div>
          </div>
        </div>
      </li>
      {% endfor %}
    </ol>
  </div>
  {% endfor %}

  <p class="scholar-link">
    <a href="{{ site.google_scholar }}" target="_blank" rel="noopener">Any discrepancy? Refer to my Google Scholar</a>.
  </p>
</div>
