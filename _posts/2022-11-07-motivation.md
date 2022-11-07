---
layout: post
title: Motivation 
permalink: /motivation/
---

Our knowledge about the history of life on Earth is humanity’s shared heritage. The analyses of databases that archive this knowledge has become a cornerstone of modern paleontological/evolutionary research, which is crucially dependent on computational infrastructure and human resources.
 
1. We support the establishment of an open, global organisation that ensures that data provision for paleontological/evolutionary research is robust, openly accessible, unbiased, equitable and sustainable. 

2. We support the establishment of an openly-developed, community-owned, internationally-organised data lake that aims at integrating data from existing databases, published literature and museum/institutional collections. The data service is expected to support previously untestable scientific hypotheses by increasing the spatiotemporal coverage of the fossil record and providing specimen-level data of global coverage.

3. We support that the organisation (1) be responsible for the management, curation and the organisation of the next generation of data service to be used in paleontological/evolutionary research.

  Open Science Collaboration

### List of Members

{% for person in site.data.supporters %}

{% if person['webpage']%}

[**{{person['prefix']}} {{person['first_name']}} {{person['last_name']}} {{person['suffix']}}**]({{person['webpage']}}) - {{person['institute']}}, {{person['country']}}

{% else %}

**{{person['prefix']}} {{person['first_name']}} {{person['last_name']}} {{person['suffix']}}** - {{person['institute']}}, {{person['country']}}

{% endif %}

{% endfor %}


