<p align="center">
<img src="https://3u26hb1g25wn1xwo8g186fnd-wpengine.netdna-ssl.com/files/2019/06/mozilla-logo-bw-rgb-1024x293.png" alt="Mozilla logo" width="180"/>
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
      <td>{{ app.authors }}</td>
      <td>{{ app.status }}</td>
    </tr>
  {% endfor %}
  </tbody>
</table>