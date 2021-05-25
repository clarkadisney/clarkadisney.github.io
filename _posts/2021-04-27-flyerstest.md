---
layout: projectpost
title: Flyers Test
date: 2019-03-25T11:32:43.215Z
categories: [Artwork]
tags: [Flyers, Punk, Louisville]
featured-image: /assets/images/artwork/flyers1.JPG
caption: Louisville Show Flyers 1998-2004
description: 
---

# Test

<a data-fancybox="gallery" href="/assets/images/artwork/flyers1.JPG">
<img class="projectimage" src="/assets/images/artwork/flyers1.JPG"></a>

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