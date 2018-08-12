---
layout: page
title: Beers
---

We are still developing and refining our recipes before production begins towards the end of the year. 
Below we have a sampling of things to come.

{% for beer in site.data.beers.core %}
<h2>{{ beer.name }}</h2>
<div class="row"><div class="col-sm-8">
{{ beer.description }}
</div><div class="col-sm-4">
{% if beer.image %}
<img class="img-responsive" src="{{ beer.image }}">
{% endif %}
</div></div>
{% endfor %}

# Coming soon...

{% for beer in site.data.beers.soon %}
<h2>{{ beer.name }}</h2>
<div class="row"><div class="col-sm-8">
{{ beer.description }}
</div><div class="col-sm-4">
{% if beer.image %}
<img class="img-responsive" src="{{ beer.image }}">
{% endif %}
</div></div>
{% endfor %}


