---
layout: page
title: Beers
---

{% for beer in site.data.beers.core %}
<h2>{{ beer.name }}</h2>
<div class="row">
{% if beer.image %}
<div class="col-sm-8">
{{ beer.description }}
</div><div class="col-sm-4">
<img class="img-responsive" src="{{ beer.image }}"></div>
{% else %}
<div class="col-sm-12">
{{ beer.description }}
</div>
{% endif %}
</div>
{% endfor %}


# Coming soon...

{% if site.data.beers.soon %}
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
{% else %}
More exciting beers in development!
{% endif %}


