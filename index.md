---
#
# By default, content added below the "---" mark will appear in the home page
# between the top bar and the list of recent posts.
# To change the home page layout, edit the _layouts/home.html file.
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
#
layout: home
---
## Programming foundations

These are the foundations of all programming. While the syntax of programming languages may be different, they all use the same foundations.

<dl>
{% for example in site.foundations %}
  <dt><a href="{{example.permalink}}">{{ example.title }}</a></dt>
  <dd>{{example.summary}}</dd>
{% endfor %}
</dl>

## Examples
<dl>
{% for example in site.examples %}
  <dt><a href="{{example.permalink}}">{{ example.title }}</a></dt>
  <dd>{{example.summary}}</dd>
{% endfor %}
</dl>