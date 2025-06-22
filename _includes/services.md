## Misc.

<h4 style="margin:0 10px 0;">Experience</h4>

<ul style="margin:0 0 5px;">
{% for role in site.data.experience.main %}
  <li>{{ role.title }} @ <i>{{ role.company }}</i> ({{ role.period }})</li>
{% endfor %}
</ul>

<h4 style="margin:0 10px 0;">Conference Reviewers</h4>

<ul style="margin:0 0 5px;">
  <li><a href="https://aclrollingreview.org/"><autocolor>ACL Rolling Review (ARR) 2025</autocolor></a></li>
  <li><a href="https://www.nlpcc2025.org/"><autocolor>Natural Language Processing and Chinese Computing (NLPCC) 2025</autocolor></a></li>
</ul>