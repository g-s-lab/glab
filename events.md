---
layout: page
title: Events
permalink: /events/
---

# Events


<div>
  <ul class="event-list">
    {% for post in site.categories['events'] %}
    <li>
      <span class="post-meta">{{ post.date | date: "%b %-d, %Y, %l:%M %p" }} • {{ post.name }} {% if post.categories contains 'Homotop2015' %}  • (Homotopical Structures Seminar) {% endif %} {% if post.categories contains 'Hodge2016' %}   • (Hodge Theory Seminar) {% endif %}  </span>
      <br>
      <a class="event-link" href="{{ post.url | prepend: site.baseurl }}">
        {{ post.title }}
      </a>
      </br>
      </br>
    </li>
    {% endfor %}
  </ul>
</div>
