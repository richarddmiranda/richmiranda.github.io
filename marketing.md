---
layout: page
title: 
permalink: /marketing/
---

<div class="posts">



<div class="cat-nav">
  <ul>
    <li>
      <a  href="/articles">Show All</a>
    </li>
    <li>
    <a  href="/entrepreneurship" class="btn-nav">Entrepreneurship</a>
          </li>
    <li>
      <a class="is-active" href="/marketing" >Marketing</a>
    </li>
    <li>
      <a href="/parenting" class="btn-nav">Parenting</a>
    </li>
    
  </ul>
</div>

  

  {% for post in site.categories.marketing %}
  <!-- {% unless post.categories contains "notes" or post.categories contains "lists"%} -->
    <article class="post">

      <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h1>

      <div class="entry">
        {{ post.excerpt }}
      </div>

      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More</a>
    </article>
  <!-- {% endunless %} -->
  {% endfor %}


