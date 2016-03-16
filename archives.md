---
layout: default
permalink: /archives
---

<div class="home">

  <header class="post-header">
    <h1 class="post-title">Posts</h1>
  </header>
  <!-- <h1 class="page-heading">Posts</h1> -->

  <ul class="archive-list">
    {% for post in site.posts %}
      <li>
        <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span> &raquo;  <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>        
      </li>
    {% endfor %}
  </ul>
  <p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>
</div>