---
layout: post
title: i'm going to try to put some code here in Jupyter
date: 2023-12-24 08:57:00-0400
description: this is an attempt by me to use this website (dangerous)
tags: jupyter, python
categories: posting
giscus_comments: true
related_posts: false
---

To include a jupyter notebook in a post, you can use the following code:

{% raw %}

```html
{::nomarkdown}
{% assign jupyter_path = "assets/jupyter/blog.ipynb" | relative_url %}
{% capture notebook_exists %}{% file_exists assets/jupyter/blog.ipynb %}{% endcapture %}
{% if notebook_exists == "true" %}
    {% jupyter_notebook jupyter_path %}
{% else %}
    <p>Sorry, the notebook you are looking for does not exist.</p>
{% endif %}
{:/nomarkdown}
```