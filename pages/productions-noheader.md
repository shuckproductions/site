---
layout: noheader
title: Productions HIDE
permalink: /productions-sans-header/
menu: main
---
<base target="_parent" />
<br>
<div class="grid-container">

{% for post in site.categories.production %}
<a href="{{post.url}}">
<div class="grid-33 mobile-grid-100 blockhome">
<div class="attop">
  <img class="largeimage" style="background:url('{% if post.largeimage %}{{site.baseurl}}/image/{{post.largeimage}}{% else %}{{site.baseurl}}/image/productions/comingsoon.png{% endif %}');"><br>
	</div>	 
	  <div class="atbottom"><div class="panel-heading panelhead-prods">{{ post.title }}</div>
	 </div>
	 </div>
</a>

{% endfor %}

</div>




