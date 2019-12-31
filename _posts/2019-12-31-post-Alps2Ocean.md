---
title: "Alps2Ocean - a self guided tour in the South Island New Zealand"
author: emma
categories:
  - albums
tags:
  - cycle
  - 2019-NZ
day0gallery:
  - image_path: /assets/albums/2019-12-31-post-Alps2Ocean/day0-1.JPEG
    url:  /assets/albums/2019-12-31-post-Alps2Ocean/day0-1.JPEG
    alt: "Jd riding along the Pukaki flats"
    title: "Jd riding along the Pukaki flats"
  - image_path: /assets/albums/2019-12-31-post-Alps2Ocean/day0-2.JPEG
    url:  /assets/albums/2019-12-31-post-Alps2Ocean/day0-2.JPEG
    alt: "Em riding along the Pukaki flats"
    title: "Em riding along the Pukaki flats"
  - image_path: /assets/albums/2019-12-31-post-Alps2Ocean/day0-3.JPEG
    url:  /assets/albums/2019-12-31-post-Alps2Ocean/day0-3.JPEG 
    alt: "A muffin break at Lake Pukaki"
    title: "A muffin break at Lake Pukaki"
  - image_path: /assets/albums/2019-12-31-post-Alps2Ocean/day0-4.JPEG
    url:  /assets/albums/2019-12-31-post-Alps2Ocean/day0-4.JPEG
    alt: "Jd and Em  at Lake Pukaki (windy!)"
    title: "Jd and Em  at Lake Pukaki (windy!)"
---

Our first and last blog post for 2019 - we promise to do better in 2020!

Date: 2019 December 27th to 2020 January 1st

Alps 2 Ocean official website: <https://www.alps2ocean.com/>

## Map of route

<link rel="stylesheet" href="https://unpkg.com/leaflet@1.5.1/dist/leaflet.css"
   integrity="sha512-xwE/Az9zrjBIphAcBb3F6JVqxf46+CDLwfLMHloNu6KEQCAWi6HcDUbeOfBIptF7tcCzusKFjFw2yuvEpDL9wQ=="
   crossorigin=""/>  

<script src="https://unpkg.com/leaflet@1.5.1/dist/leaflet.js"
   integrity="sha512-GffPMF3RvMeYyc1LWMHtK8EbPv0iNZ8/oTtHPx9/cc2ILxQ+u905qIwdpULaqDkyBKgOaB57QTMg7ztg8Jm2Og=="
   crossorigin=""></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/leaflet-gpx/1.4.0/gpx.min.js"></script>

<div id="mapid" style="width: 80%; height: 400px;"></div>
<script>

var mymap = L.map('mapid').setView([44.112664, 5.407952], 13);

L.tileLayer( 'http://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
    attribution: '&copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a>',
    subdomains: ['a','b','c']
}).addTo( mymap );

var gpx = 'https://www.jdem.com.au/assets/albums/2019-07-11-post-sault-lavender-cycle/2019-07-11-post-sault-lavender-cycle.gpx';

new L.GPX(gpx, {async: true,   marker_options: {
    startIconUrl: '/assets/images/pin-icon-start.png',
    endIconUrl: '/assets/images/pin-icon-end.png',
    shadowUrl: '/assets/images/pin-shadow.png'
  }}).on('loaded', function(e) { mymap.fitBounds(e.target.getBounds()); }).addTo(mymap);
</script>

## 2019 Dec 27 - Day 0 False start (Twizel to Lake Pukaki return)

{% include gallery id="day0gallery" layout="half" caption="Photos from Twizel to Lake Pukaki return." %}

 We were off to a false start this morning as the helicopter flying over the tasman (river) was prevented from flying due to high winds and low cloud cover. We postponed the start of the tour by a day and cycled to Lake Pukaki instead.

### Highlights

- Our second cycle ride since leaving France in July (seriously) had us wondering if we were cut out for the days ahead.
- A much needed muffin break 10 kilometres in provided the much (not) needed sustenance for the 45 min cycle back.
- Neither of us had ever seen lakes fed by glaciers, surrounded by mountains, and water was a beautiful blue colour (apparently due to [glacial flour](<https://en.wikipedia.org/wiki/Rock_flour>)).
- Jd coined a new term for a phenomenon he had witnessed over the last few years: *'over-weathering: the process by which Emma reads too much into the weather forecasts for the days ahead, including visiting multiple different meteorological sources for the same locations'*. In this *single instance*, it turned that Emma's prediction of poor weather at Mt Cook for the day was correct.

### GPS Route
<div id="mapid" style="width: 100%; height: 400px;"></div>

<script>
var mymap = L.map('mapid').setView([44.112664, 5.407952], 13);

L.tileLayer( 'http://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
    attribution: '&copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a>',
    subdomains: ['a','b','c']
}).addTo( mymap );

var gpx = 'https://www.jdem.com.au/assets/albums/2019-12-31-post-Alps2Ocean/2019-12-27_Day_0_Twizel_LakePukaki.gpx';

new L.GPX(gpx, {async: true,   marker_options: {
    startIconUrl: '/assets/images/pin-icon-start.png',
    endIconUrl: '/assets/images/pin-icon-end.png',
    shadowUrl: '/assets/images/pin-shadow.png'
  }}).on('loaded', function(e) { mymap.fitBounds(e.target.getBounds()); }).addTo(mymap);
</script>


## Day 1 Mt Cook Village to Twizel

## Day 2 Lake Ohau Lodge to Omarama

## Day 3 Omarama to Kurow via Otematata

## Day 4 Kurow to Duntroon

## Day 5 Duntroon to Oamaru