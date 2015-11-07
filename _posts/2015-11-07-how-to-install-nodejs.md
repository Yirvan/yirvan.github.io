---
layout: post
title: How to Install Nodejs on Lubuntu 14.04
description: "Best nodejs installation methode"
modified: 2015-11-07
tags: [nodejs, npm, console, javascript]
image:
  feature: abstract-10.jpg
  credit: dargadgetz
  creditlink: http://www.dargadgetz.com/ios-7-abstract-wallpaper-pack-for-iphone-5-and-ipod-touch-retina/
---

From CLI, write:


{% highlight css %}
sudo apt-get update
sudo apt-get install build-essential libssl-dev
curl https://raw.githubusercontent.com/creationix/nvm/v0.24.1/install.sh | sh
source ~/.profile
nvm ls-remote
nvm install 4.2.2
node -v
{% endhighlight %}
