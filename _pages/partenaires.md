---
title: Les Partenaires
seo_title: Partenaires
layout: collection
permalink: /partenaires/
collection: partenaires
entries_layout: grid
classes: wide
---

<div id="map" style="height: 610px; width:100%"></div>

<script>
var osm = L.tileLayer('https://tile.openstreetmap.org/{z}/{x}/{y}.png', {
    maxZoom: 19,
    attribution: '© OpenStreetMap'
});

var map = L.map('map', {
    center: [48.301404208912494, -3.7773972693157214],
    zoom: 8,
    layers: [osm]
});

{%- for unite in site.pepinieres -%}
    {% if unite.location.latitude and unite.location.longitude %}
      {% if unite.actions[0].url %}
        L.marker([ {{unite.location.latitude}}, {{unite.location.longitude}} ])
         .bindPopup(L.popup({maxWidth:500}).setContent("{{unite.title}}<br><a href='{{ unite.actions[0].url }}' target='_blank'>Lien direct</a>"))
         .addTo(map);
      {% else %}
        L.marker([ {{unite.location.latitude}}, {{unite.location.longitude}} ])
         .bindPopup(L.popup({maxWidth:500}).setContent("{{unite.title}}<br>"))
         .addTo(map);
      {% endif %}
    {% endif %}
{% endfor %}

</script>