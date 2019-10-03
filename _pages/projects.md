---
layout: page
title: Projects
permalink: /projects/
---

{% for project in site.projects %}

{% if project.redirect %}
<div class="project">
    <div class="thumbnail">
        <a href="{{ project.redirect }}" target="_blank">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img | prepend: site.baseurl | prepend: site.url }}"/>
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
{% else %}

<div class="project ">
    <div class="thumbnail">
        <a href="{{ project.url | prepend: site.baseurl | prepend: site.url }}">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img | prepend: site.baseurl | prepend: site.url }}"/>
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

{% endif %}

{% endfor %}

These are some of the projects I’ve worked on in my spare time.

## The Markdown and pandoc resume

Maintaining a resume is one of those annoying tasks that always takes up much more time than it should. Compounding this is the fact that resumes are regularly requested in different formats: raw text, pdf, Microsoft Word, etc. In addition, it might be desirable to have a HTML version online somewhere for added visibility. How then to manage this complexity? No one wants to manually update four versions of their resume, and the pdf conversion tools included with word processors leave much to be desired.
https://www.chainsawonatireswing.com/2013/05/28/how-i-create-manage-my-cv-using-markdown-pandoc/

![Sample resume](https://github.com/resume-nation/resume-nation.github.io/blob/master/images/stock-demo.PNG?raw=true)

## NetXMS tools

## Hands-On lab
### Let's Build a Home Virtualization Lab Environment - A Build Log 

![Hands-On lab](https://louwrentius.com/static/images/dl380htop01.png)
Like many people in IT, I’ve been building labs at home to be able to test things I plan on doing at work and learn new technologies in my free time.

## Administrator certifications
### EX200 — Red Hat Certified System Administrator (RHCSA)

## Virtual Data Room
