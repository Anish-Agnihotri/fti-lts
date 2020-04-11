---
layout: home
---
<p align="center">
  <a href="https://builders.mozilla.community/" target="_blank">{% include moz-logo.svg %}</a>
<h3 align="center">Fix-the-internet (S20) LTS</h3>
<h3 align="center">Collection of Mozilla Fix-the-internet (S20) applications, ideas, and long-term results.</h3>
</p>

# Applications

<table>
  <thead>
    <tr>
      <th>Team Name</th>
      <th>One-liner</th>
      <th>Members</th>
      <th>Status</th>
    </tr>
  </thead>
  <tbody>
  {% for app in site.apps %}
    <tr>
      <td><a href="{{ app.url }}">{{ app.title }}</a></td>
      <td>{{ app.description }}</td>
      <td>{% for author in app.authors %}{% if author.url %}<a href="{{author.url}}">{{author.name}}</a>{% else %}{{author.name}}{% endif %}{% if forloop.last == false %}, {% endif %}{% endfor %}</td>
      <td>{{ app.status }}</td>
    </tr>
  {% endfor %}
  </tbody>
</table>
