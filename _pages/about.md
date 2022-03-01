---
layout: about
title: about
permalink: /
# subtitle: <a href='#'>Affiliations</a>. Address. Contacts. Moto. Etc.
subtitle: <a href='#'>AI Engineer</a>.

profile:
  align: right
  image: prof_pic.jpg
  caption: >
    <i style="font-size: x-small">Generated with ArcaneGAN4</i>
  address: >
    <p>Student at CentraleSupelec</p>
    <p>+33 6 34 66 88 58</p>
    <p>m5u9s00@gmail.com</p>

news: false  # includes a list of news items
selected_projects : true
selected_papers: false # includes a list of papers marked as "selected={true}"
social: true  # includes social icons at the bottom of the page
---


Hello there :wave:

I’m Mustapha AJEGHRIR and this is my personal website. Please feel free to go through my [`projects`](/projects), you can email me if necessary.

I’m very interested in AI and its applications. I love to engineer new/classic algorithms and methods to get the best value for highly demanding applications where multiple skills are required.

## Interested in :
- Artificial Intelligence 
  - Natural Language Processing
  - Computer Vision
  - Audio
  - Tabular Data
  - Forcasting
  - Reinforcement Learning
  ...
- Mathematics
  - Modelization
  - Optimization
  - Probabilities
  - Algebra
  ...
- Software Engineering
- Full stack development


---

## Some of my projects :
See all projects here : [`projects`](/projects)

{% if page.selected_projects -%}
  <!-- Projects -->
  <div>
    {%- assign sorted_projects = site.projects | where: "selected", true | sort: "importance" -%}
    <div class="projects">  
      <div class="grid">
        {%- for project in sorted_projects -%}
        {% include projects.html %}
        {%- endfor %}
      </div>              
    </div>
  </div>
{%- endif %}
