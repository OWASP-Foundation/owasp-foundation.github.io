---

title: Flagships
displaytext: Flagship Projects
layout: null
tab: true
order: 1
tags: projects

---

## Flagship Projects
### Projects that have demonstrated strategic value to OWASP and application security as a whole

{% assign stan_projects = site.data.projects | where:'type', 'standards' | where:'level', '4' %}
{% assign tool_projects = site.data.projects | where:'type', 'tool' | where:'level', '4' %}
{% assign documentation_projects = site.data.projects | where:'type', 'documentation' | where:'level', '4' %}
{% assign code_projects = site.data.projects | where:'type', 'code' | where:'level', '4' %}
{% assign other_projects = site.data.projects | where:'type', 'other' | where:'level', '4' %}

***
### Standards Projects

{% for project in stan_projects %}
### [{{ project.title }}]({{ project.url }})
{{ project.pitch }}
{% endfor %}

### Tool Projects

{% for project in tool_projects %}
### [{{ project.title }}]({{ project.url }})
{{ project.pitch }}
{% endfor %}

### Documentation Projects 

{% for project in documentation_projects %}
### [{{ project.title }}]({{ project.url }})
{{ project.pitch }}
{% endfor %}

### Code Projects

{% for project in code_projects %}
### [{{ project.title }}]({{ project.url }})
{{ project.pitch }}
{% endfor %}

{% if other_projects.count > 0 %}
### Other Projects

{% for project in other_projects %}
### [{{ project.title }}]({{ project.url }})
{{ project.pitch }}
{% endfor %}

{% endif %}
