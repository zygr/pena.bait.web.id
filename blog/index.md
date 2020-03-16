---
layout: default
title: Penabait Blog
heading: Laman Blog Penabait
description: Foo & bar.
---
<header>
    <h1>{{ page.heading }}</h1>
</header>


  <section>
    {% for post in site.posts %}
    <header>
      <div><small>{{ post.date | date_to_string }}</small></div>
      <h3><a href="{{ post.url }}" title="{{ post.title }}">{{ post.heading }}</a></h3>
    </header>
    <hr>
    {% endfor %}
  </section>
