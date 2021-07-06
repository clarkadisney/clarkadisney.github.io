---
layout: organicspost
title: Update - No-till Bags
date: 2020-10-01T12:30:00.000Z
categories: [Organics]
tags: [Notill, Containers, Microbiome]
featured-image: /assets/images/chiroof/notill6.JPG
caption: 1, 2, and 3 month's growth
description: 
---

# Did it work?
Very well - we had a great canopy significantly faster than any previous season. The size of the crops were in some cases noticeably larger, and the formerly typical soil top-offs were reduced and - in some areas unnecessary. We had a rolling harvest that started in June/July and lasted into November.
 
We'd expected to need to add <i>something</i>, whether that be some immediately-available liquid organic nutrient - or even some mycorrhizal fungi to help with the compost breakdown. Not once was this required...not even after topping with excessive, not-finished compost and coco coir. We likely would have stuck with this method regardless due to our goal of closed-loop, but the added growth was a major bonus.
 
## One month growth
 
<a data-fancybox="gallery" href="/assets/images/chiroof/notill5.JPG"><img class="projectimage" src="/assets/images/chiroof/notill5.JPG"></a>
 
## Two month's growth
 
<a data-fancybox="gallery" href="/assets/images/chiroof/notill6.JPG"><img class="projectimage" src="/assets/images/chiroof/notill6.JPG"></a>
 
## Three month's growth
 
<a data-fancybox="gallery" href="/assets/images/chiroof/cherrypeppers.JPG"><img class="projectimage" src="/assets/images/chiroof/cherrypeppers.JPG"></a>
 
<a data-fancybox="gallery" href="/assets/images/chiroof/notill11.JPG"><img class="projectimage" src="/assets/images/chiroof/notill11.JPG"></a>
 
<a data-fancybox="gallery" href="/assets/images/chiroof/notill7.JPG"><img class="projectimage" src="/assets/images/chiroof/notill7.JPG"></a>
 
<a data-fancybox="gallery" href="/assets/images/chiroof/notill8.JPG"><img class="projectimage" src="/assets/images/chiroof/notill8.JPG"></a>
 
## Selected Harvest
 
<a data-fancybox="gallery" href="/assets/images/chiroof/food1.JPG"><img class="projectimage" src="/assets/images/chiroof/food1.JPG"></a>
 
<a data-fancybox="gallery" href="/assets/images/chiroof/food2.JPG"><img class="projectimage" src="/assets/images/chiroof/food2.JPG"></a>
 
<a data-fancybox="gallery" href="/assets/images/chiroof/food3.JPG"><img class="projectimage" src="/assets/images/chiroof/food3.JPG"></a>
 
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
