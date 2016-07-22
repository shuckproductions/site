---
layout: page
title: Blog
menu: main
permalink: /blog/
---

<div class="grid-container">

<div class="grid-30 mobile-grid-100" style="height:520px;">
<a class="twitter-timeline" data-width="300" data-height="500" data-theme="light" data-link-color="#2B7BB9" href="https://twitter.com/shuckproduction">Tweets by shuckproduction</a> <script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>
</div>


{% for post in site.categories.blog  %}
 <div class="grid-30 mobile-grid-100">
<div class="panel-heading">{{ post.title }}</div>
<p>{{ post.excerpt | strip_html | truncatewords:25 }}</p>
 <a href="{{ post.url }}" class="btn btn-default">Read more</a> <a class="panel-date">{{ post.date | date: '%B %d, %Y' }}</a><br>
</div>

{% endfor %}
</div>