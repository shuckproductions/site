---
layout: page
title: Testimonials
permalink: /testimonials/
navigation_weight: 4
menu: main
---

<div class="grid-container gridbox">
<br>
{% for post in site.categories.testimonial %}
<div class="grid-100 mobile-grid-100 gridtestimonial">
<div class="grid-container">
	<div class="leftside grid-30 mobile-grid-100 noline grid-left"><br>
		<div class="testimonialimage" style="background:url('{{site.baseurl}}/image/{{post.logo}}');"></div>
		<span class="testimonialtitle">{{ post.title }}</span><br>
		<span class="testimonialmonthyear">{{post.monthyear}}</span>
	</div>
	<div class="rightside grid-60 mobile-grid-100 grid-right noline">
		<span class="testimonialkeytext">"{{post.keytext}}"</span><br>
		<span class="testimonialcontent">{{post.content}}</span>
	</div>
</div>
</div><br>

{% endfor %}
