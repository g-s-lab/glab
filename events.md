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
      <span class="post-meta">{{ post.date | date: "%b %-d, %Y, %l:%M %p" }} • {{ post.name }} • {{ post.tags }} </span>
      <br>
      <a class="event-link" href="{{ post.url | prepend: site.baseurl }}">
        {{ post.title }}
      </a>
      </br>
    </li>
    {% endfor %}
  </ul>
</div>
