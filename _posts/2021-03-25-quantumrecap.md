---
layout: projectpost
title: Quantum Recap
date: 2021-03-25T00:30:00.000Z
categories: [plants]
tags: [Growrack]
featured-image: /assets/images/analysis/LEDcalc.JPG
caption: Very recent history of LED grow lights
description: 
---
 
# Quantum Board Recap
 
Grow light marketing is awash with misinformation, and the <a href="https://horticulturelightinggroup.com/pages/the-quantum-board-project" target="_blank" rel="noopener noreferrer">niche </a> crowd tends to <a href="https://cre.science/en/lm301h-vs-lm301b/#comments" target="_blank" rel="noopener noreferrer">lead</a> adoption (subject to diode availability). For this group the 2010s to current acceptance of "best" grow light has gone: "blurple" -> "COB" -> "Quantum Board." Reasons frequently cited for this shift include: deceptive marketing of power draw "at the fixture," changes to <a href="https://www.ledsmagazine.com/horticultural-lighting/article/16695503/experts-examine-plant-response-to-ssl-and-market-potential-at-horticultural-conference-magazine" target="_blank" rel="noopener noreferrer">understanding</a> of how plants absorb light, and the availability of high efficiency diodes - namely <a href="https://www.samsung.com/led/lighting/mid-power-leds/3030-leds/lm301h/" target="_blank" rel="noopener noreferrer">Samsung's.</a>
 
The point of this post is to highlight recent reductions (~15yrs max) in the cost of light. For a much cooler, much longer term read I highly recommend <a href="https://www.nber.org/system/files/chapters/c6064/c6064.pdf">reading</a> - or at least <a href="https://econlife.com/2018/10/the-light-side-of-economic-growth/">skimming</a>, the famous William Nordhaus study.
 
I posit that the two most important recent changes were: 
 
1. the 2019 introduction of the Samsung LM-301x diode. These diodes are more efficient by <a href="https://en.wikipedia.org/wiki/Haitz%27s_law" target="_blank" rel="noopener noreferrer">orders of magnitude</a> than those on the market a decade ago - and in particular, are nearly double the efficiency of less than 5 years ago. Not only are they more efficient in terms of Haitz's law, but they are competitively more efficient when PPFD is measured. <a href="https://ledgardener.com/lumens-par-ppf-and-ppfd-measuring-cob-grow-light-output/#:~:text=PPFD%20is%20measured%20in%20micromoles,per%20square%20meter%20or%20foot." target="_blank" rel="noopener noreferrer">Here</a> is an easy explainer of PPFD and related terminology.
 
2. The introduction of the Quantum Board, a matrix of mid-power wide-spectrum diodes. They are sold in multiples with customized and well-machined heatsinks and Meanwell drivers.
 
 
#### Sidebar - Kelvin vs Wavelength
Generalizing: When something that looks white is listed as "3500K," the 3500k is actually an <i>approximation</i> for how the combination of different wavelengths produced by the light source <i>appears</i>. This is <a href="https://physics.stackexchange.com/questions/357031/is-color-temperature-and-wavelength-the-same-thing">complicated</a> to calculate and is beyond our purpose (and my abilities).
 
#### Sidebar - Marketing
In the light fixture market wide-spectrum usually refers to the Kelvin temperature approximation of a <i>singly-packaged</i> diode that contains <i>more than one diode</i> inside the package and <i>produces multiple wavelengths.</i> This is a similar concept to a COB but not necessarily the same - it doesn't mean the diodes are mounted to silicon within the package.  
 
There are a lot of absolute claims re: spectrum, and unfortunately like any known-unknown it's where a lot of disinformation lies. Some fixture manufacturers misuse the already-subjective term "full-spectrum" with an approximated Kelvin temperature for a combination of single-wavelength diodes. This is generally frowned upon by the market and not present in serious offerings. Typically <i>all</i> manufacturers offer a chart showing the specific wavelength output of their fixture similar to the below:
 
<a data-fancybox="gallery" href="/assets/images/analysis/HLGWavelength.JPG"><img class="projectimage" src="/assets/images/analysis/HLGWavelength.JPG"></a>
 
### "Blurple"
Lights comprised primarily of far-red and blue diodes (they look purple) were originally thought to provide plants all they need. The resulting sankey-esque assumption was energy for wavelengths outside of the "photosynthesis" and "growth" ranges was wasted energy...this is no longer considered accurate. The <a href="https://www.ledsmagazine.com/horticultural-lighting/article/16695503/experts-examine-plant-response-to-ssl-and-market-potential-at-horticultural-conference-magazine" target="_blank" rel="noopener noreferrer">example</a> I chose is from an LED trade magazine, but one can easily search google scholar or scrape data from any large online forum (reddit / pushshift) and come to the same conclusion by comparing blurple and wide-spectrum results: although the green /"middle" spectrum is likely least understood in photobiology, it's definitely doing <i>something</i>:
 
<a data-fancybox="gallery" href="/assets/images/analysis/Changes.JPG"><img class="projectimage" src="/assets/images/analysis/Changes.JPG"></a>
 
Technical advances in LED diodes have led to "full-spectrum" or "multi-spectrum" lights that are still heavily-composed of far-red and blue diodes leading to a pinkish hue. <a href="https://www.osram.com/os/news-and-events/spotlights/horticulture-lighting-think-pink.jsp" target="_blank" rel="noopener noreferrer">OSRAM</a> is big here, and the fixtures are still semi-popular / marketed today. They are not always seen as a serious contender for growers - especially those alternating crops. Some companies offer <a href="https://www.lumigrow.com/smartpar-software/" target="_blank" rel="noopener noreferrer">programmability</a> to overcome this.
 
### COB
COB stands for <b>Chip On Board</b>, a reference to the diodes being mounted directly to a semiconductor. More accurately, COBs are an <i>array</i> of many diodes tightly packed and bonded on a (usually silicon) board. These fixtures are BRIGHT, and were brighter than anything on the market upon release. When arranged in an array over a growing area - despite their usually-higher power draw, they can be more efficient than blurples. They also kick off less heat, something that keeps coming up as a problem for growers at scale (but shouldn't - more on that another time). Notably, COBs are "full" or "wide" spectrum when measured in Kelvin.
 
### Quantum Board
A Quantum Board (QB) is a trade name from Horticulture Lighting Group. The fixture can be seen as an evolution of the COB. A QB still uses diodes mounted in silicon - however instead of many packed tight and bundled into a single fixture, a QB uses less-dense, mid-powered diodes and spreads 288 of them over a large single silicon board:
 
<a data-fancybox="gallery" href="/assets/images/LEDs/quantum7.JPG"><img class="projectimage" src="/assets/images/LEDs/quantum7.JPG"></a>
 
The result is a higher PPFD on average. The efficiency of this array pattern is visible in this poorly-scaled excel chart ...one could buy 5 quantum boards for less than one of the first light, pay less than 1/5 the electricity per board, and cover the same area with <i>much</i> higher PPFD and 4 "squares" to spare.
 
<a data-fancybox="gallery" href="/assets/images/analysis/LEDcalc.JPG"><img class="projectimage" src="/assets/images/analysis/LEDcalc.JPG"></a>
 
This is both in part to the shifting of the array concept to something more akin to a matrix - and certainly helped by the use of more efficient mid-power diodes.  They've been updated to include far-red and blue (in small amounts, separately), and to use the newest diodes. Although they remain among the more expensive, in 2021 there are a number of bar-shaped competitors employing a similar approach online with comparable results. The key in the fixture game is looking for independent <a href="https://cdn.shopify.com/s/files/1/1538/8585/files/HLG_650R.pdf?v=1587049529" target="_blank" rel="noopener noreferrer">lab results</a>. The funky <a href="https://en.wikipedia.org/wiki/Integrating_sphere" target="_blank" rel="noopener noreferrer">sphere</a> used to test is required for luminous flux results and is usually something a lab owns.
 
One standout from 2020 is that Samsung has begun making the silicon boards for HLG. I am not aware of what that actually <i>means</i> but perception online is that it would ensure best mounting, best flux-binned diodes (which the LMH should already be), etc.
 
### 2019 - Samsung LM301H (B)
 
 The First 2016 QB288v1 usedSamsung LM561C diodes which have been variously tested up to ~2.5 μmol/j. Current boards use the LM301H which has been widely-tested by a variety of labs at a high as ~3.1 μmol/j. This is compared to ~1.0 in the late-aughts.  
 
### 2021 - No competitors?
Similar to the spectrum charts of fixture side, diode manufacturers often make available their <a href="https://www.samsung.com/led/lighting/mid-power-leds/3030-leds/lm301h/" target="_blank" rel="noopener noreferrer">design files</a>  and technical specifications. This is currently the pound for pound winner in the diode game.
 
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
