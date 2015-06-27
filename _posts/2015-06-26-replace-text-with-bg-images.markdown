---
layout: post
title: "How to replace text with background images (HTML & SASS)."
date: {}
categories: jekyll update
published: false
---

Cara menyembunyikan text dan menggantinya dengan background-image 
(ref. codyhouse).

HTML code:

    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <title>Document</title>
        <link rel="stylesheet" href="/css/main.css">
    </head>
    <body>
        <div class="cd-item-navigation">
            <a class="cd-img-replace"href="#0">Prev</a>
        </div>
    </body>
    </html>

SASS code:

    .cd-item-navigation a //mengatur posisi icon posisi sisi-sisi di tengah ancestor element dan menyembunyikannya/display none saat awal dan akan terlihat saat mouse hover pada area tertentu.
        position: absolute
        top: 50%
        -webkit-transform: translateY(-50%)
        -moz-transform: translateY(-50%)
        -ms-transform: translateY(-50%)
        -o-transform: translateY(-50%)
        transform: translateY(-50%)
        width: 36px
        height: 66px
        background-color: rgba(216, 216, 216, 0.4)
        background-image: url("/img/cd-icon-arrow.svg")
        background-repeat: no-repeat
        background-position: center center
        z-index: 4
        display: none
        border-radius: 0.25em

    .cd-item-navigation a:hover
        background-color: rgba(216, 216, 216, 0.6) //membuat background lebih gelap saat mouse hover utk membuat kesan focus pada navigasi

    .cd-item-navigation a.visible
        display: block
        -webkit-animation: cd-fade-in 0.4s
        -moz-animation: cd-fade-in 0.4s
        animation: cd-fade-in 0.4s

    .cd-img-replace 
        /* replace text with background images, text is hiding/overflow by indent it 100% */
        display: inline-block
        overflow: hidden
        text-indent: 100%
        white-space: nowrap

[jekyll]:      http://jekyllrb.com
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-help]: https://github.com/jekyll/jekyll-help
