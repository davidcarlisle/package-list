---
title: LaTeX package tagging status
---



<table style="width:100%">
<thead>
<tr>
<th>package</th>
<th>status</th>
<th>Comments</th>
<th>Issue</th>
</tr>
</thead>
<tbody>

{%- for p in site.data.packages -%}
<tr>
<td><a href="https://ctan.org/pkg/{{p.package}}">{{p.package}}</a></td>
<td>{{p.status}}</td>
<td>{{p.comments}}</td>
<td>
{%- if p.issue -%}
<a href="https://github.com/latex3/tagging-project/issues/{{p.issue}}">#{{p.issue}}</a>
{%- endif -%}
{% if p.related-issues %}
<br/>
See also
{% for u in p.related-issues %}
<a href="https://github.com/latex3/tagging-project/issues/{{u}}">#{{u}}</a>
{% endfor %}
{% endif %}
</td>
</tr>
{%- endfor -%}

<tbody>
</table>



