---
layout: page
title: Interviews
permalink: /interviews/
---

  <ul class="post-list">
    {% for post in site.posts %}
      <li>
        <img src="{{post.image}}" class="thumb"></img>

        <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

        <h2>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        </h2>
        <p>{{ post.interviewee }}, {{ post.location }}</p>
        
        <p>{{ post.excerpt }}</p>
      </li>
    {% endfor %}
  </ul>

  <p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>
