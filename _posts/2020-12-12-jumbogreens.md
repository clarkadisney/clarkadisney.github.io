---
layout: growrackpost
title: Field-sized greens!
date: 2020-12-12T12:00:01.000Z
categories: [plants]
tags: [Growrack, Containers]
featured-image: /assets/images/greens/greens1.JPG
caption: Big leaves and yields to help get through Chicago winter!
description: 
---

# Jumbogreens
With the addition of the 1/4" egg crate, the combined aeration and humidity made for some serious growth:
 
## Root Protection
 
Added plastic mesh to keep root structure in-tact
 
<a data-fancybox="gallery" href="/assets/images/greens/greens3.JPG"><img class="projectimage" src="/assets/images/greens/greens3.JPG"></a>
 
<a data-fancybox="gallery" href="/assets/images/greens/greens4.JPG"><img class="projectimage" src="/assets/images/greens/greens4.JPG"></a>
 
## Ruby Red
 
<a data-fancybox="gallery" href="/assets/images/greens/greens1.JPG"><img class="projectimage" src="/assets/images/greens/greens1.JPG"></a>
 
<a data-fancybox="gallery" href="/assets/images/greens/greens2.JPG"><img class="projectimage" src="/assets/images/greens/greens2.JPG"></a>
 
## Curly Kale + Arugula
Same idea - aeration + irrigation. Arugula seems to be going much faster than the kale:
 
<a data-fancybox="gallery" href="/assets/images/greens/greens10.JPG"><img class="projectimage" src="/assets/images/greens/greens10.JPG"></a>
 
<a data-fancybox="gallery" href="/assets/images/greens/jumbogreensarugula.JPG"><img class="projectimage" src="/assets/images/greens/jumbogreensarugula.JPG"></a>
 
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
 
 
 

