---
layout: post
permalink: /blog/
title: blog
command: ls -l
---

### total {{ site.posts | size }}
<div class="posts">
  {% for post in site.posts %}
    <article class="post">

      <h5>{{ post.description }}</h5>

      <a href="{{ site.baseurl }}{{ post.url }}" class="link2">Read</a>
    </article>
  {% endfor %}
</div>

<hr>

