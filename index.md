---
layout: default
---

# Geometric Structures Lab

The Geometric Structures Lab is located within the [Fields Institute](http://www.fields.utoronto.ca/) at the [University of Toronto](http://www.math.toronto.edu/) and engages in basic research at the interface of mathematics and physics.  Main focus areas include [generalized geometry](https://en.wikipedia.org/wiki/Generalized_complex_structure), [Poisson geometry](https://en.wikipedia.org/wiki/Poisson_manifold), the [Hitchin system](https://en.wikipedia.org/wiki/Hitchin_system), the theory of [Lie groupoids](https://en.wikipedia.org/wiki/Lie_groupoid), the exact WKB method, the [Riemann-Hilbert correspondence](https://en.wikipedia.org/wiki/Riemann%E2%80%93Hilbert_correspondence) and the study of [quantum field theory](https://en.wikipedia.org/wiki/Quantum_field_theory).

  A primary function of the Laboratory is to support and enhance the training of graduate and undergraduate students. To this end, we organize meetings to discuss and explain our research, as well as master classes given by invited experts.

{% assign counter = 0 %}
{% for post in site.categories['talk'] %}
  {% capture nowunix %}{{'now' | date: '%s'}}{% endcapture %}
  {% capture posttime %}{{post.date | date: '%s'}}{% endcapture %}
  {% if posttime > nowunix %}
    {% assign counter = counter | plus: 1 %}                
  {% endif %}
{% endfor %}
      
{% if counter != 0 %}
## Upcoming Events  
{% endif %}

<div class="home">
  <ul class="post-list">
  {% assign counter = 0 %}
  {% assign curDate = site.time | date: '%s' %}
  {% for post in site.categories['talk'] reversed %}
    {% assign postStartDate = post.date | date: '%s' %}
    {% if postStartDate >= curDate and counter  < 5 %}
       {% assign counter = counter | plus: 1 %}                
         <li>
           <span class="post-meta">{{ post.date | date: "%b %-d, %Y, %-T" }}</span>
            <h2>
               <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.name }}, {{ post.title }}</a>
           </h2>
         </li>
        
    {% endif %}
{% endfor %}
  
</ul>


  <!-- <p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>
 -->
</div>
