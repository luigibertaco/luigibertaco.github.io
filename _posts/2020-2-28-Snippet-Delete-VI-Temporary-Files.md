---
layout: post
title: Snippet - Delete VI temporary files
---

The following bash command will delete all `*.un~` files recursivelly.

{% highlight bash %}
find . -type f -name '*.un~' -delete
{% endhighlight %}
