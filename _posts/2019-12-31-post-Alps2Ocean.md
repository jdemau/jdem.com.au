---
title: "Alps2Ocean - a self guided tour in the South Island New Zealand"
author: emma
categories:
  - albums
tags:
  - cycle
  - 2019-NZ
day0gallery:
  - image_path: /assets/albums/2019-12-31-post-Alps2Ocean/day0-1.jpg
    url:  /assets/albums/2019-12-31-post-Alps2Ocean/day0-1.jpg
    alt: "Jd riding along the Pukaki flats"
    title: "Jd riding along the Pukaki flats"
  - image_path: /assets/albums/2019-12-31-post-Alps2Ocean/day0-2.jpg
    url:  /assets/albums/2019-12-31-post-Alps2Ocean/day0-2.jpg
    alt: "Em riding along the Pukaki flats"
    title: "Em riding along the Pukaki flats"
  - image_path: /assets/albums/2019-12-31-post-Alps2Ocean/day0-3.jpg
    url:  /assets/albums/2019-12-31-post-Alps2Ocean/day0-3.jpg 
    alt: "A muffin break at Lake Pukaki"
    title: "A muffin break at Lake Pukaki"
  - image_path: /assets/albums/2019-12-31-post-Alps2Ocean/day0-4.jpg
    url:  /assets/albums/2019-12-31-post-Alps2Ocean/day0-4.jpg
    alt: "Jd and Em  at Lake Pukaki (windy!)"
    title: "Jd and Em  at Lake Pukaki (windy!)"
day1gallery:
  - image_path: /assets/albums/2019-12-31-post-Alps2Ocean/day1-01.jpg
    url:  /assets/albums/2019-12-31-post-Alps2Ocean/day1-01.jpg
    alt: "Jd getting ready for our first (official) riding day"
    title: "Jd getting ready for our first (official) riding day"
  - image_path: /assets/albums/2019-12-31-post-Alps2Ocean/day1-02.jpg
    url:  /assets/albums/2019-12-31-post-Alps2Ocean/day1-02.jpg
    alt: "The start of the Alps to Ocean A20"
    title: "The start of the Alps to Ocean A20"
  - image_path: /assets/albums/2019-12-31-post-Alps2Ocean/day1-03.jpg
    url:  /assets/albums/2019-12-31-post-Alps2Ocean/day1-3.jpg 
    alt: "Emma on the path between Mt Cook Village and Mt Cook Airport"
    title: "Emma on the path between Mt Cook Village and Mt Cook Airport"
  - image_path: /assets/albums/2019-12-31-post-Alps2Ocean/day1-04.jpg
    url:  /assets/albums/2019-12-31-post-Alps2Ocean/day1-04.jpg
    alt: "The helicopter taking our bikes away"
    title: "The helicopter taking our bikes away"
  - image_path: /assets/albums/2019-12-31-post-Alps2Ocean/day1-05.jpg
    url:  /assets/albums/2019-12-31-post-Alps2Ocean/day1-05.jpg
    alt: "The pilot unloads our crate of bikes"
    title: "The pilot unloads our crate of bikes"
  - image_path: /assets/albums/2019-12-31-post-Alps2Ocean/day1-06.jpg
    url:  /assets/albums/2019-12-31-post-Alps2Ocean/day1-06.jpg
    alt: "Jd and Em as we start our ride"
    title: "Jd and Em as we start our ride"
  - image_path: /assets/albums/2019-12-31-post-Alps2Ocean/day1-07.jpg
    url:  /assets/albums/2019-12-31-post-Alps2Ocean/day1-07.jpg 
    alt: "Em takes the lead"
    title: "Em takes the lead"
  - image_path: /assets/albums/2019-12-31-post-Alps2Ocean/day1-08.jpg
    url:  /assets/albums/2019-12-31-post-Alps2Ocean/day1-08.jpg
    alt: "Jd riding along the Pukaki flats"
    title: "Jd riding along the Pukaki flats"
  - image_path: /assets/albums/2019-12-31-post-Alps2Ocean/day1-09.jpg
    url:  /assets/albums/2019-12-31-post-Alps2Ocean/day1-09.jpg
    alt: "Lupins by Lake Pukaki"
    title: "Lupins by Lake Pukaki"
  - image_path: /assets/albums/2019-12-31-post-Alps2Ocean/day1-10.jpg
    url:  /assets/albums/2019-12-31-post-Alps2Ocean/day1-10.jpg
    alt: "Selfie at Lake Pukaki!"
    title: "Selfie at Lake Pukaki!"
  - image_path: /assets/albums/2019-12-31-post-Alps2Ocean/day1-11.jpg
    url:  /assets/albums/2019-12-31-post-Alps2Ocean/day1-11.jpg 
    alt: "Em at Lake Pukaki"
    title: "Em at Lake Pukaki"
  - image_path: /assets/albums/2019-12-31-post-Alps2Ocean/day1-12.jpg
    url:  /assets/albums/2019-12-31-post-Alps2Ocean/day1-12.jpg
    alt: "Tekapo B Power Station and penstock"
    title: "Tekapo B Power Station and penstock"    

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
<div id="day0map" style="width: 100%; height: 400px;"></div>
<script>
var day0map = L.map('day0map').setView([-44.2599014,170.1042942], 13);

L.tileLayer( 'http://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
    attribution: '&copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a>',
    subdomains: ['a','b','c']
}).addTo( day0map );

var gpx = 'https://www.jdem.com.au/assets/albums/2019-12-31-post-Alps2Ocean/2019-12-27_Day_0_Twizel_LakePukaki.gpx';

new L.GPX(gpx, {async: true,   marker_options: {
    startIconUrl: '/assets/images/pin-icon-start.png',
    endIconUrl: '/assets/images/pin-icon-end.png',
    shadowUrl: '/assets/images/pin-shadow.png'
  }}).on('loaded', function(e) { day0map.fitBounds(e.target.getBounds()); }).addTo(day0map);
</script>


## Day 1 Mt Cook Village to Twizel

{% include gallery id="day1gallery" layout="half" caption="Photos from My Cook Village to Twizel." %}

The weather wasa great this morning, as we took  a van transfer from Twizel to the Mt Cook Village, and cycled 6 kilometres to the Mt Cook Aiport. Our bikes were loaded into a crate, and shuttled across the Tasman (river) via helicopter (ridiculous, we know). We soon followed the bikes before commencing our journey on the other side of the  Tasman through the Mt Cook National Park.

A few photos for Emma, and a few too many photos for Jaidev, we cycled a very bumpy and rocky 12 kilometres to 'Jollies Carpark'. Emma felt she was killing it, until a well placed rock got the better of her and her bike. She was down! And (luckily) her elbow took the brunt of the fall. A quick unclip by Jaidev, providing some expert medical care ('you should drink some water'), and we were back moving.

The next 40 kilometres along Lake Pukaki were hard going, through a logging track, but the views were worth it. We enjoyed lunch by the lupins (and the bees), looking back over Lake Pukaki and Mt Cook.

We passed the Tekapo B Power Station (JD: amazing!, Em: not so much), and we were soon back at where we were yesterday on Lake Pukaki.

### Highlights

- Trail riding together was an interesting experience - fun at times, but also hard work!
- The helicopter (while a short ride) was a great way to see the Mt Cook National Park from the air.
- 80 kilometres of scenic riding was something special.
- The weather today was *fantastic* - sunny but cool.

### GPS Route

## Day 2 Lake Ohau Lodge to Omarama

## Day 3 Omarama to Kurow via Otematata

## Day 4 Kurow to Duntroon

## Day 5 Duntroon to Oamaru
