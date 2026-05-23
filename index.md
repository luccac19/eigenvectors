---
layout: default
title: Home
---

test2
# Blog Posts

{% for post in site.posts %}
  <article class="post-card">

    <h3>
      <a href="{{ post.url | relative_url }}">
        {{ post.title }}
      </a>
    </h3>

    <p>
      {{ post.date | date: "%B %-d, %Y" }}
    </p>

    <div>
      {{ post.excerpt }}
    </div>

    <p>
      <a href="{{ post.url | relative_url }}">
        Read More →
      </a>
    </p>

  </article>
{% endfor %}
