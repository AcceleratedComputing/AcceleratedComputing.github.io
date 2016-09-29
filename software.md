---
layout: default
title: Accelerated Software
permalink: /software/
---

The following software has been developed by UK Research intitions to target accelerated computing architectures. If you would like to add your software to this list then please [contact us](contact) or submit a pull request.

<div class="griditem row">
{% include software_tags.html %}
{% for i in site.data.software %}
<div class="griditem-item col-md-4 col-sm-6 col-xs-12" data-tags='{{ i.tags | jsonify | downcase }}'>
	<div class="well griditem-outer">
		<div class="griditem-inner">
			
			
			
			<div class="griditem-img bordered" style="background-image: url({% if i.image contains 'http' %}'{{ i.image }}'{% else %}'/static/img/{{ i.image }}'{% endif %});"></div>
			
			<h3 class="griditem-headlines">{{ i.name }}</h3>
			
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
				<a href="{{ i.url }}" class="btn btn-info btn-raised btn-sm griditem-link">Website</a>
				{% endif %}
			</div>
		</div>
	</div>
	</div>
{% endfor %}
</div>
 
