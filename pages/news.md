---
title: News
permalink: /news/
---

<p>Subscribe with <a href="{{ site.baseurl }}/feed.xml">RSS</a> to keep up with the latest news.</p>

{% for post in site.posts limit:10 %}
   <div class="post-preview">
<h2 style="color: #a855f7; font-weight: bold; font-size: 38px;"><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h2>
   <span class="post-date">{{ post.date | date: "%B %d, %Y" }}</span><br>
   {% if post.badges %}{% for badge in post.badges %}<span class="badge badge-{{ badge.type }}">{{ badge.tag }}</span>{% endfor %}{% endif %}
   {{ post.content | split:'<!--more-->' | first }}
   {% if post.content contains '<!--more-->' %}
      <a href="{{ site.baseurl }}{{ post.url }}">read more</a>
   {% endif %}
   </div>
   <hr>
{% endfor %}

Want to see more? See the <a href="{{ site.baseurl }}/archive/">News Archive</a>.
