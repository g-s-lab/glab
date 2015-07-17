---
layout: page
title: Blog
permalink: /blog/
---

# Blog

<ul class="post-list">
{% for post in site.categories['blog'] %}
	<li>
        <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }} • {{ post.author }}</span>
        <h3>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        </h3>
    </li>
{% endfor %}
</ul>
