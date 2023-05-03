---
layout: custom_page
title: "Portfolio"
description: "Hello! My name is Gavin, and I'm a gameplay programmer currently working on the game 'Nemesis Siege' from red9gameworks.
	This site currently serves as my portfolio, which contains various projects that I have worked on during my spare time."
---

<article class="home">
   <header class="about-header">
    <h2 class="about-title">{{ "About" | escape }}</h2>
  </header>
  
  <div class="about">
	<img class="avatar_img" src="https://avatars.githubusercontent.com/u/29388665?v=4" style="float:left" />
  
	<br>
	<br>
  
	<div class="avatar_text">
		<h1> {{ page.description }} </h1>
	</div>
	
	<br>
	<br>
  </div>
  
  <div class="projects">
	<header class="project-header">
		<h2 class="project-title">{{ "Projects" | escape }}</h2>
	</header>

	{% assign project_list = site.projects | sort: "order" %}

	{% for project in project_list %}
		<h3> <a href="{{ project.url }}"> {{ project.title }} </a> </h3>
	{% endfor %}
  </div>
</article>