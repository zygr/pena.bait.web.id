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
      <h3><span>{{ post.date | date_to_string }}</span> » <a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a></h3>
    {% endfor %}
  </section>