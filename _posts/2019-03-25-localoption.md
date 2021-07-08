---
layout: softwarepost
title: Rough Concept
date: 2019-03-25T11:32:43.215Z
categories: [Software]
tags: [Local Option, Software, Photography]
featured-image: /assets/images/localoption/rough_concept_4.JPG
caption: Standalone photo archiving solution
description: Photo archiving solution
series: [LocalOption Test]
---
# Problem addressed
My friend and I were sitting at a bar catching up...

## A walled garden
Local Option is a privacy-focused photograph management system currently in development. We believe that your memories are yours, and that your family shouldn't need to grant programatic access to your personal lives in exchange for storage and sorting features.

# Fellows of freeware's past

## Program 1
<a data-fancybox="gallery" href="/assets/images/localoption/rough_concept_1.JPG">
<img class="postimage" src="/assets/images/localoption/rough_concept_1.JPG"></a>

## Program 2
<a data-fancybox="gallery" href="/assets/images/localoption/rough_concept_2.JPG">
<img class="postimage" src="/assets/images/localoption/rough_concept_2.JPG"></a>

## Program 3
<a data-fancybox="gallery" href="/assets/images/localoption/rough_concept_3.JPG">
<img class="postimage" src="/assets/images/localoption/rough_concept_3.JPG"></a>

## Program 4
<a data-fancybox="gallery" href="/assets/images/localoption/rough_concept_4.JPG">
<img class="postimage" src="/assets/images/localoption/rough_concept_4.JPG"></a>

# The real MVP
<figure><blockquote><p><i>Local Option is a privacy-focused photograph management system currently in development. We believe that your memories are yours, and that your family shouldn't need to grant programatic access to your personal lives in exchange for storage, transfer, and sorting features.</i>

<i>No demo yet, but we expect to have something to kick the tires on in 2019. The program is currently <a href="https://github.com/pkuca/local-option" style="color: #070e36; font-weight: bolder;" target="_blank" rel="noopener noreferrer">written</a> in JavaScript, utilizes <a href="https://docs.opencv.org/3.4/df/df7/tutorial_js_table_of_contents_setup.html" style="color: #070e36; font-weight: bolder;" target="_blank" rel="noopener noreferrer">OpenCV.js</a>, and is packaged in <a href="https://www.electronjs.org/docs" style="color: #070e36; font-weight: bolder;" target="_blank" rel="noopener noreferrer">Electron</a></i></p></blockquote></figure>


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