{# receives 'issues_list', 'labels_to_issues', and 'piggy' #}

# Welcome to the {{config.site_name}}!

This page is made from `site-templates/index.md`. We should edit that!


Ask (or answer) a new question by [creating an issue](https://github.com/datalab-affiliates/resources/issues)!

## Start here!

{% for issue in issues_list %}
{% if issue.is_frontpage %}

[{{config.issue_title_prefix}}{{issue.title}}]({{issue.output_filename}})

{% endif %}
{% endfor %}

---

## [All questions](examples.md)

---

## [All categories](labels.md)
