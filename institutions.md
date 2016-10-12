---
layout: default
title: UK Institutions with Accelerated Computing Groups and Communities
permalink: /institutions/
---

<div class="griditem row">
    {% for i in site.data.institutions %}
    <div class="griditem-item col-md-4 col-sm-6 col-xs-12" data-tags='{{ i.tags | jsonify | downcase }}'>
    	<div class="well griditem-outer">
    		<div class="griditem-inner">
    			
    			<div class="griditem-img bordered" style="background-image: url({% if i.image contains 'http' %}'{{ i.image }}'{% else %}'/static/img/{{ i.image }}'{% endif %});"></div>
			
                {% if i.url %} <a  href="{{ i.url }}"> {% endif %}
    			<h3 class="griditem-headlines">{{ i.name }}</h3>
    			{% if i.url %} </a> {% endif %}
    			<div class="griditem-footer"> 
    				{% if i.url %} 
    				<a href="{{ i.url }}" class="btn btn-info btn-raised btn-sm griditem-link">{% if i.url contains 'http'%}External Link{% else %}More Details{% endif %}</a>
    				{% endif %}
    			</div>
    		</div>
    	</div>
        </div>
    {% endfor %}
</div>

If you currently run a group which focuses on the application or development of accelerated computing then please add you institution or alternatively update your existing institutional details to include your group. Changes should be proposed via Github pull request using the [following instructions](../howto/add_institution).