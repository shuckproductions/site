---
layout: page
title: Blog
permalink: /blog/
---

<div class="blocks">
<div class="postblock">

<div class="panel panel-default panel-twitter">
  <div class="panel-heading">Tweets</div>
  <div class="panel-body">
    <a class="twitter-timeline" data-width="300" data-theme="light" data-link-color="#2B7BB9" href="https://twitter.com/shuckproduction">Tweets by shuckproduction</a> <script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>
  </div>
</div> 

{% for post in site.categories.blog %}
<div class="panel panel-default panel-post">
  <div class="panel-heading">{{ post.title }}</div>
  <div class="panel-body">
	<p>{{ post.excerpt | strip_html | truncatewords:25 }}</p>


	 <a href="{{ post.url }}" class="btn btn-default">Read more</a> <a class="panel-date">{{ post.date | date: '%B %d, %Y' }}</a><br>
	 </div>

</div>
{% endfor %}
</div>
</div>