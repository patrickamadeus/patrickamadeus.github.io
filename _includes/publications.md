<a class="back-link" href="{{ '/' | relative_url }}">&larr; {{ site.title }}</a>

<h2>Publications</h2>
<p class="pub-legend">* equal contribution &middot; See also <a href="{{ site.google_scholar }}" target="_blank" rel="noopener">Google Scholar</a></p>

{% assign year_groups = site.data.publications.main | group_by: "year" | sort: "name" | reverse %}
{% for year_group in year_groups %}
<h3>{{ year_group.name }}</h3>
<ul class="pubs">
{% for pub in year_group.items %}{% include pub_item.html pub=pub %}{% endfor %}
</ul>
{% endfor %}
