---
layout: post
author: Marco Gualtieri
title: Hodge Theory Working Group
date: 2016-02-16
categories: blog
published: true
---


## Hodge Theory | winter 2016

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
