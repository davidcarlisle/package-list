---
title: LaTeX package/class tagging status
---
<style>
td.supported {background-color: #DDFFDD;font-weight:bold;}
td.partial-support {background-color: #FFFFDD;font-weight:bold;}
td.no-support {background-color: #FFDDDD;font-weight:bold;}
</style>
<script src="sorttable.js"></script>

# LaTeX Package Tagging Status

This file shows the status of LaTeX [Packages](#packages) and [Classes](#classes)
with respect to PDF tagging.

To add or edit the entries, please make a pull request to change the YAML file
[tagging-status.yml](https://github.com/davidcarlisle/package-list/blob/main/_data/tagging-status.yml).


## Packages

{%- assign packages = site.data.tagging-status | where: "type", "package" -%}
{% include_relative status-section.md %}


## Classes

{%- assign packages = site.data.tagging-status | where: "type", "class" -%}
{% include_relative status-section.md %}


----


## References


<span id="ref1">1.</span> U. Fischer and F. Mittelbach. Automated tagging of LATEX documents — what is possible today, in 2023? TUGboat, 44(2):262–266, 2023.

<span id="ref2">2.</span> F. Mittelbach and U. Fischer. Enhancing LATEX to automatically produce tagged and accessible PDF. TUGboat, ?:?, 2024. 


