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
</th>
</thead>
<tbody>
{%- for p in site.data.packages -%}
<tr>
<td>{{p.package}}</td>
<td>{{p.status}}</td>
<td>{{p.comments}}</td>
<td>{{p.issue}}</td>
</tr>
{%- endfor -%}
<tbody>
</table>



