---
layout: page
title: Beers
---

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


