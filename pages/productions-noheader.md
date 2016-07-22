---
layout: noheader
title: Productions
permalink: /productions-sans-header/
---

<div class="grid-container">

{% for post in site.categories.production %}
<div class="grid-30 mobile-grid-100">
  <div class="panel-heading">{{ post.title }}</div>
  <img class="tinyimage" src="{{site.baseurl}}/image/{{post.tinyimage}}"><br>
  <p class="minorinfo"><b><i class="fa fa-calendar" aria-hidden="true"></i> Produced:</b>{{ post.date | date: "%B %Y" }}<br></p>
	<p class="minorinfo"><b><i class="fa fa-check-square" aria-hidden="true"></i>  Skills: </b>{{ post.skills }} </p>
	 <div class="atbottom"><a href="{{ post.url }}" class="btn btn-default">Read more</a></div>
	 </div>


{% endfor %}

</div>




