---
layout: growrackpost
title: Roots?
date: 2020-12-10T13:15:00.000Z
categories: [Growrack]
tags: [Containers, LEDs]
featured-image: /assets/images/growrack/rackroots7.JPG
caption: Moving past greens and herbsdispd
description: 
---

# Growrack root vegetable initial experiments
 
## Beets in 3601 plastic
 
Came out predictably stunted - will redo in square bags or fabric tray liners.
 
<a data-fancybox="gallery" href="/assets/images/growrack/rackroots3.JPG"><img class="projectimage" src="/assets/images/growrack/rackroots3.JPG"></a>
 
<a data-fancybox="gallery" href="/assets/images/growrack/rackroots2.JPG"><img class="projectimage" src="/assets/images/growrack/rackroots2.JPG"></a>
 
<a data-fancybox="gallery" href="/assets/images/growrack/rackroots1.JPG"><img class="projectimage" src="/assets/images/growrack/rackroots1.JPG"></a>
 
## Carrots in 1/4 Gallon Round bags
 
Stunted and got fat due to 1/4" layer of perlite on bottom (initially planted for wicking - not needed). Flavorful and otherwise great, will redo densely in an array in square bags or fabric tray liners
 
<a data-fancybox="gallery" href="/assets/images/growrack/rackroots6.JPG"><img class="projectimage" src="/assets/images/growrack/rackroots6.JPG"></a>
 
<a data-fancybox="gallery" href="/assets/images/growrack/rackroots5.JPG"><img class="projectimage" src="/assets/images/growrack/rackroots5.JPG"></a>
 
<a data-fancybox="gallery" href="/assets/images/growrack/rackroots7.JPG"><img class="projectimage" src="/assets/images/growrack/rackroots7.JPG"></a>
 
## Brussel sprouts in SWICK
 
Stunted initially in 3601 plastic - switched to 1/4" fabric and appears to be doing better
 
<a data-fancybox="gallery" href="/assets/images/growrack/rackroots10.JPG"><img class="projectimage" src="/assets/images/growrack/rackroots10.JPG"></a>
 
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
