---
layout: base.liquid
---

This is some test text to see whether things are working! 

And in general, to see how we're finding 11ty so far.

{% for post in collections.posts reversed %}
  <a href="{{ post.url }}">
    <h2>{{ post.data.title }}</h2>
    <time>{{ post.data.date | date: "%B %d, %Y" }}</time>
  </a>
{% endfor %}