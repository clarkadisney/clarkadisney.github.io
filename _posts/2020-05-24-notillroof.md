---
layout: organicspost
title: No-till Bags?
date: 2020-05-24T12:30:00.000Z
categories: [Organics]
tags: [Notill, Containers, Microbiome]
featured-image: /assets/images/chiroof/notillcover.JPG
caption: Closed-Loop Effort
description: 
---

# What is no-till?
No-till is simply avoiding digging (not tilling/aerating) and in our case avoiding added nutrients. The exact definitions of no-till, vertical-till, etc. are beyond scope and scale here - the takeaway is simply that it's an approach of initially structuring your soil to allow a thriving microbial ecosystem - and then maintaining the structural and microbial integrity of that soil. Other names for this "are no-dig" or "layered" or "lasagna," sometimes the soil is called "living soil" or "hot soil" (although that can also refer to bagged live soil).
 
# Why "no-till" beds?
More specifically - why did we choose this method vs other methods known to do well in urban lots such as the "biodynamic" <a href="https://en.wikipedia.org/wiki/French_intensive_gardening">French intensive</a>? The simple answer is that it's the best fit for our scenario for the below reasons:
 
## Organics on steroids
Organics likely taste better because of microbial activity. No-till is the most microbial intensive form of growing we are aware of.
 
## Zone 5b and specific microclimate
We already have a limited season due to Chicago's location in <a href="https://planthardiness.ars.usda.gov/PHZMWeb/">USDA Zone 5b</a>. This conflicts with our desire for both longer growing chiles in the <i>Caspacium Chinese</i> species, as well as our desire to have a double harvest in some slots where we initially plant fast-growing crops. No-till stands firm as one of the fastest organic methods that doesn't involve the constant pouring of additional nutrients.
 
Aside from this, we have a microclimate on our rooftop that can see temperature and wind fluctuations far beyond ground level on any given day. The best defense against this is hot soil, and a strong root system - both of which are defining characteristics of no-till. 
 
## Lazy closed loop
The part about not adding nutrients was a lie, you'll eventually need to "recharge" your soil by feeding the subsurface microbiome. This can be accomplished by topping with compost...we have lots of compost and are looking to explore home biomass. Additionally, the idea of just tossing that on top and that's it (within reason) - is appealing. 
 
# What did we do 
Built 4 layers of soil into a large container and densely.
 
## Containers with stratified soil
We used a large synthetic fabric raised bed and some additional 15-25 gallon smart pots.
 
<a data-fancybox="gallery" href="/assets/images/chiroof/notill2.JPG"><img class="projectimage" src="/assets/images/chiroof/notill2.JPG"></a>
 
There are some on the market specifically for this purpose - used often in California cannabis growing. The only benefit we saw for this application were features employed to hold moisture (strips of nonporous fabric on the sides - or the inverse). This is great for preventing dry soil - which is a must, but we’re more concerned with drainage due to rainfall and thus went with a normal 2 x 2 x 12 foot Smart Pot. 
 
...Plus, we'll be greedy and plant so densely that there <i>should</i> be a pretty large canopy shading the soil - a borrowed tactic from the aforementioned French Intensive method.
 
## Layer 1
The bottom layer is usually composed of cardboard or something similar to block weeds or roots from coming into the bed - but we are using a grow bag on a chicago roof so this is not necessary. 
 
## Layer 2
For <i>this</i> first layer, we placed a large quantity of Majesty Palm leaves we had in varying stages of dryness awaiting the composter. Palm leaves are very slow to break down and in this case are replacing a more commonly-used log. We also included all of the twigs on the roof and in the gutters from neighboring trees.
 
<a data-fancybox="gallery" href="/assets/images/chiroof/majesty.JPG"><img class="projectimage" src="/assets/images/chiroof/majesty.JPG"></a>
 
## Layer 3
Next, we mixed in a healthy layer of compost and a good bit of fresh kitchen scraps. Normally you tranche this repeatedly - but we were a bit sloppy to begin with and especially by the end.
 
## Layer 4
Finally, we topped with Fox Farms Ocean Forest, an organic soil designed for containers. We mixed in a significant amount of leftover perlite (we've mostly stopped using it). This layer will allow us to plant immediately, and the perlite will help hold moisture on the top 1/4 of the soil that is most at risk for dehydration.
 
<a data-fancybox="gallery" href="/assets/images/chiroof/cocoperlite.JPG"><img class="projectimage" src="/assets/images/chiroof/cocoperlite.JPG"></a>
 
## Planted
 
<a data-fancybox="gallery" href="/assets/images/chiroof/notill3.JPG"><img class="projectimage" src="/assets/images/chiroof/notill3.JPG"></a>
 
We planted <i>very</i> densely often 3 or even 4 plants per 2x2ft cell. We're confident that this can be managed through manipulating the growth, and that we'll get the required large canopy this way.
 

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
