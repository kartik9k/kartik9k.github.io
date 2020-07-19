---
layout: page
title: artwork
permalink: /artwork/
---

{% for project in site.artwork %}

<!-- {% if project.redirect %}
<div class="project">
    <div class="thumbnail">
        <a href="{{ project.redirect }}" target="_blank">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}    
        <span>
            <h1>{{ project.title }}</h1>
            <br/>
            <p>{{ project.description }}</p>
        </span>
        </a>
    </div>
</div>
{% else %} -->

<div class="project_art ">
    <div class="thumbnail_art">
        <div class="img_row">
            <a href="{{ site.baseurl }}{{ project.url }}">
            {% if project.img %}
            <img class="thumbnail_art" src="{{ project.img }}"/>
            {% else %}
            <div class="thumbnail_art blankbox"></div>
            {% endif %}    
            <span>
                <h1>{{ project.title }}</h1>
                <br/>
                <p>{{ project.description }}</p>
            </span>
            </a>
        </div>
    </div>
</div>

<!-- {% endif %} -->

{% endfor %}
