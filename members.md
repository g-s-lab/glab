---
layout: page
title: Members
permalink: /members/
---

# Current members

### Principal Investigator

<ul class="member-list">
{% for post in site.categories['pi'] %}
    <li>
     <!--    <span class="post-meta">{{ post.desc }}</span> -->
        <h2>
          <a class="member-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.name }}</a>
        </h2>
    </li>
{% endfor %}
</ul>

### Postdocs

<ul class="member-list">
{% for post in site.categories['postdoc'] %}
  	<li>
        <!-- <span class="post-meta">{{ post.desc }}</span> -->
        <h2>
          <a class="member-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.name }}</a>
        </h2>
    </li>
{% endfor %}
</ul>

### Graduate Students

<ul class="member-list">
{% for post in site.categories['gradstu'] %}
    <li>
        <!-- <span class="post-meta">{{ post.desc }}</span> -->
        <h2>
          <a class="member-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.name }}</a>
        </h2>
    </li>
{% endfor %}
</ul>



# Alumni

<ul class="member-list">
{% for post in site.categories['alumni'] %}
  	<li>
        <!-- <span class="post-meta">{{ post.desc }}</span> -->
        <h2>
          <a class="member-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.name }}</a>
        </h2>
    </li>
 {% endfor %}
</ul>
