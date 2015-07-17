---
layout: page
title: Events
permalink: /events/
---

# Events

Video of gLab events is archived by the Fields Live system [here](http://www.fields.utoronto.ca/video-archive/event/136/2015?access_code=GeoStr)

<div>
<ul class="event-list">
{% for post in site.categories['talk'] %}
	<li>
        <span class="post-meta">{{ post.date | date: "%b %-d, %Y, %l:%M %p" }}</span>
        <h3>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">
              {{ post.name }}: <i>{{ post.title }}</i>
          </a>
        </h3>
    </li>
{% endfor %}
</ul>
</div>
