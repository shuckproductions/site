---
layout: page
title: Productions
permalink: /productions/
---

<div class="blocks">
<div class="postblock">

<div class="blocks">
<div class="postblock">

{% for post in site.categories.production %}
<div class="panel panel-default panel-production">
  <div class="panel-heading">{{ post.title }}</div>
  <div class="panel-body">
  <img class="tinyimage" src="{{site.baseurl}}/image/{{post.tinyimage}}"><br>
  <p class="minorinfo"><b><i class="fa fa-calendar" aria-hidden="true"></i> Produced:</b>{{ post.date | date: "%B %Y" }}<br>
	<p class="minorinfo"><b><i class="fa fa-check-square" aria-hidden="true"></i>  Skills: </b>{{ post.skills }} </p>
	 <a href="{{ post.url }}" class="btn btn-default">Read more</a>
	 </div>

</div>

</div>

{% endfor %}
</div>



