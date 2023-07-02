---
permalink: /sports/
title: "Video Sports Analytics"
excerpt: "This is a page not in th emain menu"
author_profile: true
redirect_from:
  - "/sports_analytics/" 
  - "/sports.html"
---

Our goal is to develop algorithms that can fully comprehend a sports game based on visual data and to create cutting-edge applications from them. To achieve this, we employ a range of artificial intelligence techniques such as computer vision, audio processing, and machine learning. We have primarily focused on basketball and football soccer due to its visual complexity and its unique challenges in terms of understanding both individual and collective actions of the players.

<style>
  td {
    border: 1px solid white;
  }
</style>

<table style="text-align: left; width: 900px; font-size: 0.9em; border: 1px solid white;" cellspacing="2" cellpadding="10" border="0">
      <tbody>
{% for p in site.data.sports %}
<tr>
  <td valign="top"><br></td>
  {% if p.project %}
  <td valign="top"><a href="{{ p.project }}"><img moz-do-not-send="true" src="{{ p.image }}" border="0" width="200" height="250"></a><br></td>
  {% else %}
  <td valign="top"><img moz-do-not-send="true" src="{{ p.image }}" border="0" width="200" height="250"><br></td>
  {% endif %}

  <td valign="top"><br></td>
  <td valign="middle"><b>{{ p.title }}</b><br>
  {{ p.authors }}<br>
  {{ p.venue }} {{ p.year }}<br>
  {% if p.pdf %}
    [<a moz-do-not-send="true" href="{{ p.pdf }}">pdf</a>]
  {% endif %}
  {% if p.project %}
    [<a moz-do-not-send="true" href="{{ p.project }}">project</a>]
  {% endif %}
  {% if p.code %}
    [<a moz-do-not-send="true" href="{{ p.code }}">code</a>]
  {% endif %}
  {% if p.demo %}
    [<a moz-do-not-send="true" href="{{ p.demo }}">demo</a>]
  {% endif %}
  {% if p.data %}
    [<a moz-do-not-send="true" href="{{ p.data }}">data</a>]
  {% endif %}
  <br>
  <font></font>
</td>
</tr>

<tr>
  <td valign="top"><br></td>
  <td valign="top"><br></td>
  <td valign="top"><br></td>
  <td valign="middle"><font face="Arial" size="-1"><br></font></td>
</tr>
{% endfor %}
</tbody>
</table>