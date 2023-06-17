---
title: Proyectos
---
<h1>Proyectos realizados</h1>
<br>
<br>
<br>

<ul>
  {% for post in site.posts %}
    <li>
      <h2 ><a href="{{ post.url }}">{{ post.title }}</a></h2>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>