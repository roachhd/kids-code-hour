---
layout: page
title: Hour of Code Resources
---

{% for page in site.posts %}
  {% if post.categories contains 'Resources' %}
    <div class="item">
      <h3><a href="/uni/{{ post.url }}">
        {{ post.title }}
      </a></h3>


<p>{{post.description}}</p>  
    </div>


  {% endif %}
{% endfor %}


{% for page in site.pages %}
  {% if page.categories contains 'Resources' %}
    <div class="item">
      <h3><a href="/uni/{{ page.url }}">
        {{ page.title }}
      </a></h3>


<p>{{page.description}}</p>  
    </div>


  {% endif %}
{% endfor %}
