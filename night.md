---
layout: page
title: Night Out
permalink: /night/
---



<div class="row">
{% for post in site.posts %}
	{% for category in post.categories %}
		{% if category == "night" %}
			<div class="col-xs-12 col-sm-6 col-md-6 col-lg-6">
		      <h1><a href="{{ post.url }}">{{ post.title }}</a></h1>
		      <p>
		        <span>{{ post.date }}</span>
		      </p>
		      <div>
        		<img class="main-post-image" src="/images/{{post.image}}" alt="Post Image">
      		  </div>
		      <div>
		        {{ post.excerpt }}
		      </div>
		    </div>
		{% endif %}
	{% endfor %}
{% endfor %}
</div>