---
layout: post
permalink: /blog
title: blog
command: ls -l
---

### total {{ site.posts | size }}
<div class="posts">
  {% for post in site.posts %}
    <article class="post">

      <h5>{{ post.title }}</h5>

      <div class="entry">
        {{ post.excerpt }}
      </div>

      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More</a>
    </article>
  {% endfor %}
</div>

<hr>

