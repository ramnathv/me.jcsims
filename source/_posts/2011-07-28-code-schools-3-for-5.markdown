---
layout: post
title: "Code School's 3 for 5"
date: 2011-07-28 11:30
comments: true
categories: [html5, css3, education, web]
---

I went through Code School's [Functional HTML5 and CSS3][1] class last night, and it was pretty awesome.  I don't have an extensive background in HTML or CSS, but I was able to pick up enough from the videos and slides to speed through it.

Read on for a cool example.

<!--more-->

Here's a small example of some awesome CSS that you get to write as part of the challenges:

{% gist 1111001 squishy_button.css %}

when combined with a simple button:

{% codeblock squishy_button.html %}
<link href='/stylesheets/squishy_button.css' rel='stylesheet' type='text/css'> 
<div>
  <a href="#" class="button"><span>Do Not Press This Button</span></a>
</div>
{% endcodeblock %}

That results in this:

{% render_partial partials/squishy_button.html %}

[1]: http://www.codeschool.com/courses/functional-html5-css3