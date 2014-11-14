---
layout: page
title: Artists
permalink: /artists/
---

<div class="home">

  <ul class="post-list">
    {% for artist in site.artists %}
    <li>
      {% if artist.featured_image %}
      <img src="/assets/artist/{{ artist.slug}}/200.png" class="featured-image" />
      {% endif %}
      <h2>
        <a class="post-link" href="{{ artist.url | prepend: site.baseurl }}">{{ artist.title }}</a>
      </h2>
    </li>
    {% endfor %}
  </ul>

</div>
