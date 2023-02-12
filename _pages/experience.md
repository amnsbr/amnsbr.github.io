---
layout: page
permalink: /experience/
title: experience
description:
nav: true
order: 2
additional_education: true
---



<div class="timeline">
  <div class="outer">
    {% for entry in site.data.experience %}
    <div class="timeline-card">
      <div class="timeline-info">
        <h4 class="timeline-title">{{entry.title}}</h4>
        <h5>{{entry.location}}</h5>
        <h6>{{entry.time}}</h6>
        <p style="color: black;">{{entry.details}}</p>
      </div>
    </div>
    {% endfor %}
  </div>
</div>

{% if page.additional_education -%}
## Courses and Workshops
<div class="row">
  <div class="education col-sm-12">
	<ol>
		{% assign sorted_courses = site.data.courses | sort: "year" | reverse %}
		{% for entry in sorted_courses %}
		<li>		
			<b>{{entry.title}}</b> ({{entry.duration}}), <!--{{entry.location}},-->{{entry.year}}
		    <!-- <span class="links">
		      {% if entry.content %}
		      [<a class="featured_content">content</a>]
		      {% endif %}
		      {% if entry.link %}
		      [<a href="{{entry.link}}" class="course_link">course page</a>]
		      {% endif %}
		      {% if entry.audit %}
		      [<a class="audit">audit only</a>]
  		      {% elsif entry.certificate %}
		      [<a href="{{ entry.certificate | prepend: '/assets/pdf/' | relative_url }}" target="_blank" class="certificate">certificate</a>]
		      {% endif %}
		    </span>
		    {% if entry.content %}
	        <span class="featured_content hidden">
	    	  <p>{{entry.content}}</p>
			</span>
			{% endif %} -->
		</li>
		{% endfor %}
	</ol>
  </div>
</div>
{%- endif %}