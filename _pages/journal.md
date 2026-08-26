---
title: ""
layout: home
permalink: /journal/
author_profile: false
---

<div class="florilegium-page">

  <header class="florilegium-page-header">

    <h1>The Journal</h1>

    <p class="page-subtitle">
      Essays · Literary quotes · Letters to you, dear Reader
    </p>

    <div class="florilegium-rule"></div>

  </header>


  <div class="florilegium-page-intro">

    <p>
      Welcome to the Journal, where you will find the raw materials of the newsletter (From the Florilegium). I might also post extra content here.
    </p> 

    <p>
        
    </p>

  </div>

<section class="florilegium-newsletter">

  <h2>Begin the correspondence</h2>

  <p>
    If you'd like to recieve the free newsletter in your inbox, please sign up by typing your email below, or follow @ambersflorilegium on Substack.
  </p>

  <iframe src="https://ambersflorilegium.substack.com/embed?transparent=1" width="480" height="320" style="border: 0; background: transparent" frameborder="0" scrolling="no"></iframe>



</section>

<section class="florilegium-journal-entries">

  <div class="florilegium-rule"></div>

  <h2>Journal Entries</h2>

  <div class="journal-entry-list">

    {% for post in site.posts %}
      <article class="journal-entry">

        <h3>
          <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        </h3>

        <p class="journal-date">
          {{ post.date | date: "%-d %B %Y" }}
        </p>

        {% if post.excerpt %}
          <div class="journal-excerpt">
            {{ post.excerpt }}
          </div>
        {% endif %}

        <a class="journal-read-more" href="{{ post.url | relative_url }}">
          Read more →
        </a>

      </article>
    {% endfor %}

  </div>

</section>