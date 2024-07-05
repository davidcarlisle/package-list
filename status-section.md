
Click on the column headings to sort the table by the chosen column.

<table class="sortable" style="min-width:100%;width:100%">
<thead>
<tr>
<!-- <th>Type</th>  -->
<th>Name</th>
<th>Status</th>
<th>Comments</th>
<th>Relevant issue</th>
<th>Team tasks</th>
<th>Last updated</th>
</tr>
</thead>
<tbody>



{%- for p in packages -%}
<tr>
<!-- <td>{{p.type}}</td> -->
<td class="{{p.status}}"><a href="https://ctan.org/pkg/{{p.name}}">{{p.name}}</a></td>
<td class="{{p.status}}">{{p.status}}</td>
<td>{{p.comments | markdownify}}</td>
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
<td>{{p.tasks}}</td>
<td>{{p.updated}}</td>
</tr>
{%- endfor -%}

</tbody>
</table>
