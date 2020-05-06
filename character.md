---
pagination:
  data: characters
  alias: character
  size: 1
layout: layouts/cinnamon.njk
permalink: "/characters/{{character.name|slug}}/"
title: Rick & Morty Characters
---

## {{character.name}}

![{{character.name}}]({{character.image}})

{% if pagination.href.previous %}
<a href="{{pagination.href.previous}}">Previous Page</a>
{% endif %}
{% if pagination.href.next %}
<a href="{{pagination.href.next}}">Next Page</a>
{% endif %}
