---
layout: post
title: jQuery in console
description: "Cara menggunakan jquery didalam console web."
modified: 2015-11-07
tags: [jquery, console, javascript]
image:
  feature: abstract-10.jpg
  credit: dargadgetz
  creditlink: http://www.dargadgetz.com/ios-7-abstract-wallpaper-pack-for-iphone-5-and-ipod-touch-retina/
---

Jalankan <code>script</code> dibawah ini pada command console browser anda:


{% highlight css %}
var script = document.createElement('script');script.src = "https://ajax.googleapis.com/ajax/libs/jquery/2.1.4/jquery.min.js";document.getElementsByTagName('head')[0].appendChild(script);
{% endhighlight %}
