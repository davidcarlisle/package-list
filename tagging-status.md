---
title: LaTeX package/class tagging status
---
<style>
td.supported {background-color: #DDFFDD;font-weight:bold;}
td.partial-support {background-color: #FFFFDD;font-weight:bold;}
td.no-support {background-color: #FFDDDD;font-weight:bold;}
</style>
<script src="sorttable.js"></script>

# Tagging Status of LaTeX Packages and Classes

This file shows the status of LaTeX [Packages](#packages) and [Classes](#classes)
with respect to PDF tagging.

The values in the *Status* column have the following meaning:

- `supported` This package or class works without any issues when tagging is enabled. If there are problems, please open an issue in [the tagging-project repo](https://github.com/latex3/tagging-project/issues).
- `partial-support` The package or class is partially supported, but some parts may not work. See comments for details.
- `currently-incompatible` The package or class is currently incompatible with the tagging code, but we expect it to be updated eventually. 
- `no-support` This package or class or class is incompatible with the tagging code and we do *not* believe that it will ever be supported.
- `unknown` The status of this package or class is not known, because there aren't reliable tests yet. Help with testing to determine the real status is very much appreciated.


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


