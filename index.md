---
layout: default
---

{% for post in site.posts %}
  <h2>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
  </h2>
  <p class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</p>
  <p>{{ post.excerpt }}</p>
{% endfor %}
