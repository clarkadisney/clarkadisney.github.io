---
layout: softwarepost
title: Rough Concept
date: 2019-03-25T11:32:43.215Z
categories: [Software]
tags: [Local Option, Software, Photography]
featured-image: /assets/images/localoption/walled_garden.JPG
caption: Idea for photo archiving solution
description: Photo archiving solution
series: [LocalOption Test]
---
# Problem

Local Option is a privacy-focused photograph management system currently in development. We believe that your memories are yours, and that your family shouldn't need to grant programatic access to your personal lives in exchange for storage and sorting features.</i>

## Testing and decision to abandon

# UI Test
<a data-fancybox="gallery" href="/assets/images/localoption/walled_garden.JPG">
<img class="postimage" src="/assets/images/localoption/walled_garden.JPG"></a>

# OpenCV.JS on Gorilla pictures :)
<a data-fancybox="gallery" href="/assets/images/localoption/log.JPG">
<img class="postimage" src="/assets/images/localoption/log.JPG"></a>

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