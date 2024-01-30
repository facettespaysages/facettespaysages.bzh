---
title: Les Partenaires
seo_title: Partenaires
layout: splash
permalink: /partenaires/
header:
  overlay_image: /assets/images/partenaires/partenaires.webp
  overlay_filter: 0.1
---

<div id="map" style="height: 610px; width:100%"></div>

<script>
var osm = L.tileLayer('https://tile.openstreetmap.org/{z}/{x}/{y}.png', {
    maxZoom: 19,
    attribution: '© OpenStreetMap'
});

var map = L.map('map', {
    center: [48.301404208912494, -3.7773972693157214],
    zoom: 9,
    layers: [osm]
});

var svg = '<svg xmlns="http://www.w3.org/2000/svg" height="16" width="14" viewBox="0 0 448 512"><!--!Font Awesome Free 6.5.1 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free Copyright 2024 Fonticons, Inc.--><path fill="#0c3922" d="M210.6 5.9L62 169.4c-3.9 4.2-6 9.8-6 15.5C56 197.7 66.3 208 79.1 208H104L30.6 281.4c-4.2 4.2-6.6 10-6.6 16C24 309.9 34.1 320 46.6 320H80L5.4 409.5C1.9 413.7 0 419 0 424.5c0 13 10.5 23.5 23.5 23.5H192v32c0 17.7 14.3 32 32 32s32-14.3 32-32V448H424.5c13 0 23.5-10.5 23.5-23.5c0-5.5-1.9-10.8-5.4-15L368 320h33.4c12.5 0 22.6-10.1 22.6-22.6c0-6-2.4-11.8-6.6-16L344 208h24.9c12.7 0 23.1-10.3 23.1-23.1c0-5.7-2.1-11.3-6-15.5L237.4 5.9C234 2.1 229.1 0 224 0s-10 2.1-13.4 5.9z"/></svg>'; /* insert your own svg */
var treeUrl = 'data:image/svg+xml;base64,' + btoa(svg);
var svg = '<svg xmlns="http://www.w3.org/2000/svg" height="16" width="16" viewBox="0 0 512 512"><!--!Font Awesome Free 6.5.1 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free Copyright 2024 Fonticons, Inc.--><path fill="#304591"  d="M469.3 19.3l23.4 23.4c25 25 25 65.5 0 90.5l-56.4 56.4L322.3 75.7l56.4-56.4c25-25 65.5-25 90.5 0zM44.9 353.2L299.7 98.3 413.7 212.3 158.8 467.1c-6.7 6.7-15.1 11.6-24.2 14.2l-104 29.7c-8.4 2.4-17.4 .1-23.6-6.1s-8.5-15.2-6.1-23.6l29.7-104c2.6-9.2 7.5-17.5 14.2-24.2zM249.4 103.4L103.4 249.4 16 161.9c-18.7-18.7-18.7-49.1 0-67.9L94.1 16c18.7-18.7 49.1-18.7 67.9 0l19.8 19.8c-.3 .3-.7 .6-1 .9l-64 64c-6.2 6.2-6.2 16.4 0 22.6s16.4 6.2 22.6 0l64-64c.3-.3 .6-.7 .9-1l45.1 45.1zM408.6 262.6l45.1 45.1c-.3 .3-.7 .6-1 .9l-64 64c-6.2 6.2-6.2 16.4 0 22.6s16.4 6.2 22.6 0l64-64c.3-.3 .6-.7 .9-1L496 350.1c18.7 18.7 18.7 49.1 0 67.9L417.9 496c-18.7 18.7-49.1 18.7-67.9 0l-87.4-87.4L408.6 262.6z"/></svg>'
var penRulerUrl = 'data:image/svg+xml;base64,' + btoa(svg);
var svg = '<svg xmlns="http://www.w3.org/2000/svg" height="16" width="20" viewBox="0 0 640 512"><!--!Font Awesome Free 6.5.1 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free Copyright 2024 Fonticons, Inc.--><path fill="#dc7e11" d="M288 48c0-26.5 21.5-48 48-48h96c26.5 0 48 21.5 48 48V192h40V120c0-13.3 10.7-24 24-24s24 10.7 24 24v72h24c26.5 0 48 21.5 48 48V464c0 26.5-21.5 48-48 48H432 336c-26.5 0-48-21.5-48-48V48zm64 32v32c0 8.8 7.2 16 16 16h32c8.8 0 16-7.2 16-16V80c0-8.8-7.2-16-16-16H368c-8.8 0-16 7.2-16 16zm16 80c-8.8 0-16 7.2-16 16v32c0 8.8 7.2 16 16 16h32c8.8 0 16-7.2 16-16V176c0-8.8-7.2-16-16-16H368zM352 272v32c0 8.8 7.2 16 16 16h32c8.8 0 16-7.2 16-16V272c0-8.8-7.2-16-16-16H368c-8.8 0-16 7.2-16 16zm176-16c-8.8 0-16 7.2-16 16v32c0 8.8 7.2 16 16 16h32c8.8 0 16-7.2 16-16V272c0-8.8-7.2-16-16-16H528zM512 368v32c0 8.8 7.2 16 16 16h32c8.8 0 16-7.2 16-16V368c0-8.8-7.2-16-16-16H528c-8.8 0-16 7.2-16 16zM224 160c0 6-1 11-2 16c20 14 34 38 34 64c0 45-36 80-80 80H160V480c0 18-15 32-32 32c-18 0-32-14-32-32V320H80c-45 0-80-35-80-80c0-26 13-50 33-64c-1-5-1-10-1-16c0-53 42-96 96-96c53 0 96 43 96 96z"/></svg>'
var treeCityUrl = 'data:image/svg+xml;base64,' + btoa(svg);

var greenIcon = new L.Icon({
  iconUrl: treeUrl,
  iconSize: [25, 41],
  iconAnchor: [12, 41],
  popupAnchor: [1, -34],
  shadowSize: [41, 41]
});

var orangeIcon = new L.Icon({
  iconUrl: treeCityUrl,
  iconSize: [25, 41],
  iconAnchor: [12, 41],
  popupAnchor: [1, -34],
  shadowSize: [41, 41]
});

var blueIcon = new L.Icon({
  iconUrl: penRulerUrl,
  iconSize: [25, 41],
  iconAnchor: [12, 41],
  popupAnchor: [1, -34],
  shadowSize: [41, 41]
});

var facetteIcon = new L.Icon({
  iconUrl: '/assets/images/favicons/logo.webp',
  iconSize: [44, 44],
  iconAnchor: [12, 41],
  popupAnchor: [1, -34],
  shadowSize: [41, 41]
});

L.marker([48.301404208912494, -3.7773972693157214], {icon: facetteIcon})
         .bindPopup(L.popup({maxWidth:500}).setContent("Facettes Paysages"))
.addTo(map);

{%- for unite in site.pepinieres -%}
    {% if unite.location.latitude and unite.location.longitude %}
      {% if unite.header.actions[0].url %}
        L.marker([ {{unite.location.latitude}}, {{unite.location.longitude}} ], {icon: greenIcon})
         .bindPopup(L.popup({maxWidth:500}).setContent("{{unite.title}}<br><a href='{{ unite.header.actions[0].url }}' target='_blank'>Lien direct</a>"))
         .addTo(map);
      {% else %}
        L.marker([ {{unite.location.latitude}}, {{unite.location.longitude}} ], {icon: greenIcon})
         .bindPopup(L.popup({maxWidth:500}).setContent("{{unite.title}}<br>"))
         .addTo(map);
      {% endif %}
    {% endif %}
{% endfor %}

{%- for unite in site.partenaires -%}
    {% if unite.incubator == "maitres_ouvrage" %}
      icon = orangeIcon;
    {% else %}
      icon = blueIcon;
    {% endif %}
    {% if unite.location.latitude and unite.location.longitude %}
      {% if unite.header.actions[0].url %}
        L.marker([ {{unite.location.latitude}}, {{unite.location.longitude}} ], {icon: icon})
         .bindPopup(L.popup({maxWidth:500}).setContent("{{unite.title}}<br><a href='{{ unite.header.actions[0].url }}' target='_blank'>Lien direct</a>"))
         .addTo(map);
      {% else %}
        L.marker([ {{unite.location.latitude}}, {{unite.location.longitude}} ], {icon: icon})
         .bindPopup(L.popup({maxWidth:500}).setContent("{{unite.title}}<br>"))
         .addTo(map);
      {% endif %}
    {% endif %}
{% endfor %}

</script>