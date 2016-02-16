---
layout: page
title: Reading Seminar
permalink: /reading/
---

# Reading Seminars

[Hodge Theory &#124; winter 2016](#Hodge2016)
<br>
[Homotopical Structures &#124; winter 2015](#Homotop2015)
<br>
[Generalised Complex Geometry &#124; autumn 2014](#GCG2014)


## <a name="Hodge2016"></a>Hodge Theory &#124; winter 2016

### Materials

[J. Carlson, S. Muller-Stach, and C. Peters, *Period Mappings and Period Domains*](http://www.cambridge.org/ca/academic/subjects/mathematics/geometry-and-topology/period-mappings-and-period-domains)
<br>
[D. Huybrechts, *Complex Geometry*](http://www.springer.com/us/book/9783540212904)

### Talks

<div>
  <ul class="event-list">
   {% for post in site.categories['reading'] %}
   {% if post.categories contains 'Hodge2016' %} 
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

## <a name="Homotop2015"></a>Homotopical Structures &#124; winter 2015

### Materials

[N. Nikolaev, *Seminar Notes*](https://www.dropbox.com/s/e6vv40kpocw37tx/Homotopical%20Structures%20Seminar.pdf?dl=0)

### Talks

<div>
  <ul class="event-list">
   {% for post in site.categories['reading'] %}
   {% if post.categories contains 'Homotop2015' %} 
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

## <a name="GCG2014"></a>Generalised Complex Geometry &#124; autumn 2014

### Materials

### Talks

<div>
  <ul class="event-list">
   {% for post in site.categories['reading'] %}
   {% if post.categories contains 'GCG2014' %} 
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