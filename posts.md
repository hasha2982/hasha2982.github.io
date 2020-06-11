---
layout: default
---

# Posts

## Latest posts

{% for post in site.posts limit:5 %}

### [{{ post.title }}]({{ post.url }})

{{ post.date | date: "%B %d, %Y" }}

{% if forloop.last == false %}

* * *

{% endif %}

{% endfor %}

## All posts

{% for post in site.posts %}

* [{{ post.title }}]({{ post.url }})

{% endfor %}
