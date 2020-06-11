---
layout: default
---

# Hi there

I'm [hasha2982](https://github.com/hasha2982), and as you can see in this site description, I am Python 3 and JavaScript developer.
You can have a look at my projects [here](/projects/index.html).

## Blog

{% for post in site.posts limit:5 %}

### [{{ post.title }}]({{ post.url }})

{{ post.date | date: "%B %d, %Y" }}

{% if forloop.last == false %}

* * *

{% endif %}

{% endfor %}

[All Posts](/posts.html#all-posts)
