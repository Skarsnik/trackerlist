---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---

{% for pack in site.data.result %}
<table>
<tr>  <td>Name: </td> <td>{{ pack[1].name }}</td> <td>Author: </td><td>{{ pack[1].author }}</td></tr>
<tr>  <td>Game: </td> <td colspan=3>{{ pack[1].game }}</td> </tr>
<tr>  <td>Download: </td><td colspan=3><a href="{{ pack[1].version_url }}">click me</a></td></tr>
</table>
{% endfor %}
