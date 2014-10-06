---
layout: page
title: Artists
permalink: /artists/
---

<div class="home">

  <h1 class="page-heading">Artists</h1>

  <ul class="post-list">
    {% for artist in site.artists %}
      <li>
      	{% if artist.featured_image %}
	<img src="/assets/thumbnails/200/{{artist.featured_image}}" class="featured-image" />
	{% endif %}
        <h2>
          <a class="post-link" href="{{ artist.url | prepend: site.baseurl }}">{{ artist.title }}</a>
        </h2>
      </li>
    {% endfor %}
  </ul>

</div>
