---
layout: post
title: Snippet - Delete VI temporary files
categories: [blog, snippets]
tags: [vi, bash]
---

The following bash command will delete all `*.un~` files recursivelly.

{% highlight bash %}
find . -type f -name '*.un~' -delete
{% endhighlight %}
