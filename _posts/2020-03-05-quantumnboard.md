---
layout: projectpost
title: Assembling QB288 3500k 
date: 2020-03-05T8:00:00.000Z
categories: [plants]
tags: [Growrack, LEDs, Products, Companies]
featured-image: /assets/images/LEDs/quantum5.JPG
caption: Samsung LM561C, 2.36 - 2.90 μmoles/joule at Board (55C)
description: Inspired by Peter Konjoian
---
<a href='/growrack.html' style="text-decoration: none; font-weight: bolder;" class='breadcrumb'> < Back To GrowRacks</a>

# HLG QB288 3500k w/ Meanwell
This is the intended light for the Growrack v2

### Fancy Heatsink  
<a data-fancybox="gallery" href="/assets/images/LEDs/quantum2.JPG">
<img class="projectimage" src="/assets/images/LEDs/quantum2.JPG"></a>

### Waygo Connectors
<a data-fancybox="gallery" href="/assets/images/LEDs/quantum4.JPG">
<img class="projectimage" src="/assets/images/LEDs/quantum4.JPG"></a>

### Extra-waterproof!
<a data-fancybox="gallery" href="/assets/images/LEDs/quantum6.JPG">
<img class="projectimage" src="/assets/images/LEDs/quantum6.JPG"></a>

### Molex Lite on the board
<a data-fancybox="gallery" href="/assets/images/LEDs/quantum5.JPG">
<img class="projectimage" src="/assets/images/LEDs/quantum5.JPG"></a>

Also, Mean Well 60H-54a Driver on the bottom!

## Aggressively Bright!
<a data-fancybox="gallery" href="/assets/images/growrack/rackv2_4">
<img class="projectimage" src="/assets/images/growrack/rackv2_4.JPG"></a>

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