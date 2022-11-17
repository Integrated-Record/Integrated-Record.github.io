---
layout: post
title: Motivation 
permalink: /motivation/
---

Our knowledge about the history of life on Earth is humanity’s shared heritage. The analyses of databases that archive this knowledge have become a cornerstone of modern paleontological/evolutionary research, which is crucially dependent on computational infrastructure and human resources.
 
1. We support the establishment of an open, global organisation that ensures that data provision for paleontological/evolutionary research is robust, openly accessible, unbiased, equitable and sustainable. 

2. We support the establishment of an openly-developed, community-owned, internationally-organised data lake that aims at integrating data from existing databases, published literature and museum/institutional collections. The data service is expected to support previously untestable scientific hypotheses by increasing the spatio-temporal coverage of the fossil record and providing specimen-level data of global coverage.

3. We support that the organisation (1) be responsible for the management, curation and the organisation of the next generation of data service to be used in paleontological/evolutionary research.

Open Science Collaboration



<div style="text-align:right">
  Open Science Collaboration
</div>

<br>

<div style="text-align:center">
<a class="btn btn-success btn-lg get-started-btn" href="https://forms.gle/JbTzFR1ZkmsborsS9">
Do you want to join and support us? 
</a>
</div>

<br>

# Open Science Collaboration 

  

### I. Endorsing databases

<div style="display:grid;grid-template-rows:auto">

{% for db in site.data.databases %}

<div style="grid-row;margin-top:10px;margin-bottom:10px">

<a href="{{db['webpage']}}">
<img src="{{site.baseurl}}{{site.url}}/images/logos/{{db['logo']}}" alt="{{db['database']}} logo" height="100px" style="margin-left:20px;margin-right:20px">
<strong>{{db['database']}}</strong>
</a>

</div>

{% endfor %}

</div>

### II. List of Members

{% assign supporters = site.data.supporters | sort : 'last_name' %}

{% for person in supporters %}

{% if person['webpage']%}

[<strong>{{person['prefix']}} {{person['first_name']}} {{person['last_name']}} {{person['suffix']}}</strong>]({{person['webpage']}}) - {{person['institute']}}, {{person['country']}}

{% else %}

<strong>{{person['prefix']}} {{person['first_name']}} {{person['last_name']}} {{person['suffix']}}</strong> - {{person['institute']}}, {{person['country']}}

{% endif %}

{% endfor %}



