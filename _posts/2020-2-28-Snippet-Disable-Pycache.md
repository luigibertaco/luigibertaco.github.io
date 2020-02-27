---
layout: post
title: Snippet - Disable pycache and remove existing folders from project
categories: [blog, snippets]
tags: [python, bash]
---

Delete pycache from project:

{% highlight bash %}
find . -type f -name '*.py[co]' -delete -o -type d -name __pycache__ -delete
{% endhighlight %}

Disable `__pycache___` creation using ENV (environmental variable):

{% highlight bash %}
export PYTHONDONTWRITEBYTECODE=1
{% endhighlight %}

or call python with `-B` parameter.

{% highlight bash %}
python -B my_python_script.py
{% endhighlight %}
