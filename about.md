---
layout: page
title: About
---

<p class="message">
  Nosy lil' fella aren't ya?
</p>

This is my github page. Theme credit goes to [@mdo](http://hyde.getpoole.com).

I'm a programmer, musician, illustrator, unicorn, yidi yada...

Currently working with [Goodhum](https://goodhum.com/). We're pretty cool, we do cool stuff, check us out.

## Tech stack

<div class="techstack-wrapper">
  {% for image in site.data.techstack %}
    <a href="{{ image.link }}">
      <img class="techstack-img" src="/public/images/{{ image.src }}" alt="image" />
    </a>
  {% endfor %}
</div>
