---
layout: softwarepost
title: Local Option Wireframe
date: 2020-03-25T11:32:43.215Z
categories: [Software]
tags: [LocalOption, Electron, OpenCV]
featured-image: /assets/images/localoption/electron_user_interface.JPG
caption: Full clickable wireframe
description: Photo archiving solution
series: [LocalOption Test]
---

# Original Mission and Wireframe

<a data-fancybox="gallery" href="/assets/images/localoption/electron_user_interface.png">
<img class="projectimage" src="/assets/images/localoption/electron_user_interface.png"></a>

<i>Local Option is a privacy-focused photograph management system currently in development. We believe that your memories are yours, and that your family shouldn't need to give marketers intimate access to your personal lives in exchange for storage and sorting features.</i>

<i>No demo yet, but we expect to have something to kick the tires on in 2019. The program is currently written in JavaScript, utilizes openCV.js, and is packaged in Electron.</i>

<i>Below are some teaser screenshots, please check for updates:</i>

## Testing and decision to abandon

# UI Test
<a data-fancybox="gallery" href="/assets/images/localoption/localUI_1.JPG">
<img class="projectimage" src="/assets/images/localoption/localUI_1.JPG"></a>

# OpenCV.JS on Gorilla pictures :)
<a data-fancybox="gallery" href="/assets/images/localoption/log.JPG">
<img class="projectimage" src="/assets/images/localoption/log.JPG"></a>

It worked!

{% assign hasSimilar = '' %}
{% for post in site.related_posts %}
{% assign postHasSimilar = false %}
{% for tag in post.tags %}
{% for thisTag in page.tags %}
{% if postHasSimilar == false and hasSimilar.size < 5 and post != page and tag == thisTag %}
{% if hasSimilar.size == 0 %}
# Similar Posts
<ul>
{% endif %}
<li class="relatedPost">
<a href="{{ site.url }}{{ post.url }}">{{ post.title }}
<img src="{{ post.featured-image }}" class='postlistimage' />
{% if post.series %}
(Series: {{ post.series }})
{% endif %}
</a>
</li>
{% capture hasSimilar %}{{ hasSimilar }}*{% endcapture %}
{% assign postHasSimilar = true %}
{% endif %}
{% endfor %}
{% endfor %}
{% endfor %}
{% if hasSimilar.size > 0 %}
</ul>
{% endif %}