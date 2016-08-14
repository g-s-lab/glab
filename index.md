---
layout: default
---

# Geometric Structures Lab

The Geometric Structures Lab is located within the [Fields Institute](http://www.fields.utoronto.ca/) at the [University of Toronto](http://www.math.toronto.edu/) and engages in basic research at the interface of mathematics and physics.  

Main focus areas include [generalized geometry](https://en.wikipedia.org/wiki/Generalized_complex_structure), [Poisson geometry](https://en.wikipedia.org/wiki/Poisson_manifold), the [Hitchin system](https://en.wikipedia.org/wiki/Hitchin_system), the theory of [Lie groupoids](https://en.wikipedia.org/wiki/Lie_groupoid), the exact WKB method, the [Riemann-Hilbert correspondence](https://en.wikipedia.org/wiki/Riemann%E2%80%93Hilbert_correspondence) and the study of [quantum field theory](https://en.wikipedia.org/wiki/Quantum_field_theory).


{% assign counter = 0 %}
{% for post in site.categories['talk'] %}
  {% capture nowunix %}{{'now' | date: '%s'}}{% endcapture %}
  {% capture posttime %}{{post.date | date: '%s'}}{% endcapture %}
  {% if posttime > nowunix %}
    {% assign counter = counter | plus: 1 %}
  {% endif %}
{% endfor %}
      
{% if counter != 0 %}
## Upcoming events  
{% endif %}

<div class="home">
  <ul class="post-list">
  {% assign counter = 0 %}
  {% assign curDate = site.time | date: '%s' %}
  {% for post in site.categories['talk'] reversed %}
    {% assign postStartDate = post.date | date: '%s' %}
    {% if postStartDate >= curDate and counter  < 3 %}
    {% assign counter = counter | plus: 1 %}
        <li>
            <span class="post-meta">{{ post.date | date: "%b %-d, %Y, %l:%M %p" }} • {{ post.name }}</span>
            <br>
                <a class="event-link" href="{{ post.url | prepend: site.baseurl }}">
                {{ post.title }}
                </a>
            </br>
        </li>
    {% endif %}
  {% endfor %}
  </ul>
</div>

## Recent events

<div class="home">
  <ul class="post-list">
{% for post in site.categories['talk'] limit: 3 %}
    <li>
        <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }} • {{ post.author }}</span>
        <h3>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        </h3>
    </li>
{% endfor %}
</ul>
</div>





<!--
## Recent blog entries  

<div class="home">
  <ul class="post-list">
{% for post in site.categories['blog'] limit: 3 %}
    <li>
        <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }} • {{ post.author }}</span>
        <h3>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        </h3>
    </li>
{% endfor %}
</ul>
</div>
-->

 





<!-- <p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>
 -->
