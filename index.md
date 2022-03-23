---
# front matter tells Jekyll to process Liquid
layout: default
my_number: 5
title: Home | Yazae.

---

## Liquid
### Objects

Objects tell liquid to output predefined variables as content
`{{ page.title }}` displays the `page.title` variable.

### Tags

Tags define the logic and control flow for templates.
```
{% if page.show_sidebar %}
  <div class="sidebar">
    sidebar content
  </div>
{% endif %}
```
This displays the sidebar if the value of the `show_sidebar` page variable is true.

### Filters

Filters change the output of a Liquid object. They are used within an output and are separated by a `|`.
For example:
`{{ "hi" | capitalize }}`
{{ "CE TEXTE SERA EN MINUSCULE" | downcase }}

This displays Hi instead of hi.

## Front matter

You can use front matter to set variables for the page:
```
---
# insert this at the top of the page
my_number: 5
---
```

and `{{ page.my_number }}` in the page :  
{{ page.my_number }}
