---
layout: default
title: Accelerated Software
permalink: /software/
---

University Accelerated Software Projects

<div class="griditem row">
{% include software_tags.html %}
{% for i in site.data.software %}
<div class="griditem-item col-md-4 col-sm-6 col-xs-12" data-tags='{{ i.tags | jsonify | downcase }}'>
	<div class="well griditem-outer">
		<div class="griditem-inner">
			<a href="/static/img/{{ i.image }}" class="thickbox">
			<div class="griditem-img bordered" style="background-image: url('/static/img/{{ i.image }}');"></div>
			</a>
			{% if i.url %} <a href="{{ i.url }}"> {% endif %}
			<h3 class="griditem-headlines">{{ i.name }}</h3>
			{% if i.url %} </a> {% endif %}
			
			<div class="griditem-content">
				<div class="tag-holder">
				{% if i.tags %} 
					{% for j in i.tags %}
					<span class="label tags tag-filter" data-tag="{{ j | downcase }}">{{ j }}</span>
					{% endfor %}
				{% endif %}
				</div>		
    		</div>
			<div class="griditem-footer"> 
				{% if i.url %} 
				<a href="{{ i.url }}" class="btn btn-info btn-raised btn-sm griditem-link">View</a>
				{% endif %}
			</div>
		</div>
	</div>
	</div>
{% endfor %}
</div>
 
