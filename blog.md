---
description: Proyectos realizados
---
<h1>Proyectos realizados</h1>
<br>

<ul>
  {% for post in site.posts %}
    {% if post.status == "done" %}
      <li>
        <h2 ><a href="{{ post.url }}">{{ post.title }}</a></h2>
        {{ post.excerpt }}
      </li>
    {% endif %}
  {% endfor %}
</ul>

<br>
<br>
<h1>Proyectos en curso</h1>
<br>

<ul>
  {% for post in site.posts %}
    {% if post.status == "WIP" %}
      <li>
        <h2 ><a href="{{ post.url }}">{{ post.title }}</a></h2>
        {{ post.excerpt }}
      </li>
    {% endif %}
  {% endfor %}
</ul>

