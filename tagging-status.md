---
title: LaTeX package/class tagging status
---
<style>
td.supported {background-color: #DDFFDD;font-weight:bold;}
</style>
<script src="sorttable.js"></script>



Click on the column headings to sort the table by the chosen column.

<table class="sortable" style="width:100%">
<thead>
<tr>
<th>Type</th>
<th>Name</th>
<th>Status</th>
<th>Comments</th>
<th>Relevant issue</th>
<th>Last updated</th>
</tr>
</thead>
<tbody>

{%- for p in site.data.tagging-status -%}
<tr>
<td>{{p.type}}</td>
<td class="{{p.status}}"><a href="https://ctan.org/pkg/{{p.name}}">{{p.name}}</a></td>
<td class="{{p.status}}">{{p.status}}</td>
<td>{{p.comments | markdownify}}</td>
<td>
{%- if p.issue -%}
<a href="https://github.com/latex3/tagging-project/issues/{{p.issue}}">#{{p.issue}}</a>
{%- endif -%}
{% if p.related-issues %}
<!-- <br/> -->
See also
{% for u in p.related-issues %}
<a href="https://github.com/latex3/tagging-project/issues/{{u}}">#{{u}}</a>
{% endfor %}
{% endif %}
</td>
<td>{{p.updated}}</td>
</tr>
{%- endfor -%}

</tbody>
</table>

----


## References


<span id="ref1">1.</span> U. Fischer and F. Mittelbach. Automated tagging of LATEX documents — what is possible today, in 2023? TUGboat, 44(2):262–266, 2023.

<span id="ref2">2.</span> F. Mittelbach and U. Fischer. Enhancing LATEX to automatically produce tagged and accessible PDF. TUGboat, ?:?, 2024. 


