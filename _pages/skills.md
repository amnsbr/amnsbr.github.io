---
layout: page
title: skills
permalink: /skills/
description:
nav: true
order: 3
---
{% for category in site.data.skills %}
<h3 style="margin-top:5px;">{{category.name}}</h3>
<div class="skills grid">
  {% assign skills = category.skills %}
  {% for skill in category.skills %}
  <div class="grid-item">
    <div class="flip-card">
    <div class="flip-card-inner">
        <div class="flip-card-front">
            <div class="skill-image-container">
                <img class="skill-image" src="{{ skill.image | prepend: '/assets/img/' | relative_url }}" alt="{{skill.image}}">
            </div>
            <div class="skill-title-container">
                <p class="skill-title">{{skill.title}}</p>
            </div>
        </div>
        <div class="flip-card-back">
            <p class="skill-desc">{{skill.description}}</p> 
        </div>
    </div>
    </div>
  </div>
  {% endfor %}
</div>
{% endfor %}
