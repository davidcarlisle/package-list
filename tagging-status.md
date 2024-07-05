---
title: LaTeX package/class tagging status
---
<style>
td.supported {background-color: #DDFFDD;font-weight:bold;}
td.unsupported {background-color: #D73A4A;font-weight:bold;}
</style>
<script src="sorttable.js"></script>

## Packages

{%- assign packages = site.data.tagging-status | where: "type", "pkg" -%}
{% include_relative status-section.md %}


## Classes

{%- assign packages = site.data.tagging-status | where: "type", "class" -%}
{% include_relative status-section.md %}


----


## References


<span id="ref1">1.</span> U. Fischer and F. Mittelbach. Automated tagging of LATEX documents — what is possible today, in 2023? TUGboat, 44(2):262–266, 2023.

<span id="ref2">2.</span> F. Mittelbach and U. Fischer. Enhancing LATEX to automatically produce tagged and accessible PDF. TUGboat, ?:?, 2024. 


