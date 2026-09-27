<p class="pub-legend">* equal contribution</p>
{% assign groups = "embodied|Embodied AI and World Models;posttraining|Multimodal Post-Training;reasoning|Multimodal Reasoning and Evaluation" | split: ";" %}
{% for g in groups %}
{% assign parts = g | split: "|" %}
{% assign items = site.data.publications.main | where: "selected", parts[0] %}
<h3>{{ parts[1] }}</h3>
<ul class="pubs">
{% for pub in items %}{% include pub_item.html pub=pub %}{% endfor %}
</ul>
{% endfor %}
