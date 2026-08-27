---
layout: single
title: ""
permalink: /devlog/
author_profile: false
---

<div class="florilegium-page">

  <header class="florilegium-page-header">

    <h1>This Website</h1>

    <p class="page-subtitle">
      GitHub Pages · Jekyll · Design
    </p>

    <div class="florilegium-rule"></div>

  </header>


  <div class="florilegium-page-intro">

    <p>
      I made this website because I wanted to create my own home on the internet, a place that can grow with me. I also wanted to be part of the <a href="https://indieweb.org/">IndieWeb</a>, which reminds me of my formative years on the Internet.
    </p> 
      You can check out my GitHub repository for the website <a href="https://github.com/ambernhafeez/ambersflorilegium">here</a>.
    <p>
        
    </p>


  </div>

<section class="devlog-intro">
  <h2>Current Development Goals</h2>
  <li>Create all project pages that currently have dead links on the site</li>
  <li>Wireframe the site to determine major design changes</li>
  <li>Design and add in orignal graphics to enhance the site's theme</li>
  <li>Flesh out the Editing and Mentoring page</li>
  <li>Flesh out the Game Dev page</li>
  <li>Flesh out the Art page</li>
</section>
  <p></p>
  <h3>Completed Goals</h3>
  <li><i>Develop functional Journal and Devlog pages with posts</i></li>
  <li><i>Create the basic site and pages based on Jekyll Minimal Mistakes</i></li>

  <section class="devlog-entries">

    <div class="florilegium-rule"></div>

    <h2>Site Notes</h2>

    <div class="devlog-entry-list">

      {% for post in site.devlog %}

        <article class="devlog-entry">

          <p class="devlog-date">
            {{ post.date | date: "%-d %B %Y" }}
          </p>

          <h3>
            <a href="{{ post.url | relative_url }}">
              {{ post.title }}
            </a>
          </h3>

          {% if post.excerpt %}
            <div class="devlog-excerpt">
              {{ post.excerpt }}
            </div>
          {% endif %}

          <a class="devlog-read-more" href="{{ post.url | relative_url }}">
            Read more →
          </a>

        </article>

      {% endfor %}

    </div>

  </section>

</div>

  <h3>Credits</h3>

  <div>The Harrington header font on this website made from <a href="https://www.onlinewebfonts.com/icon">svg icons</a> is licensed by CC BY 4.0</div>
  <p>
    The site is hosted by GitHub pages and Jekyll based on the theme Minimal Mistakes.
  </p>


