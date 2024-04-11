---
layout: post
title: CRN, ODE, and PP Examples
date: 2024-04-10 08:57:00-0400
description: A growing list of examples relating to CRNs, ODEs, PPs
tags: 
categories: 
related_posts: false
---

Download these notes here: [Examples](https://andrei-migunov.github.io/assets/jupyter/Examples.ipynb "download")

{::nomarkdown}
{% assign jupyter_path = "assets/jupyter/Examples.ipynb" | relative_url %}
{% capture notebook_exists %}{% file_exists assets/jupyter/Examples.ipynb %}{% endcapture %}
{% if notebook_exists == "true" %}
    {% jupyter_notebook jupyter_path %}
{% else %}
    <p>Sorry, the notebook you are looking for does not exist.</p>
{% endif %}
{:/nomarkdown}