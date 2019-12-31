---
title: "Alps2Ocean - Day 0 False start (Twizel to Lake Pukaki return)"
author: emma
categories:
  - albums
tags:
  - cycle
  - 2019-NZ
---

All ready to cycle day one of the Alps2Ocean trail, we were told that the helicopter was unable to fly due to poor conditions at Aoraki Mt Cook.

Date: 2019 December 27th

Distance: 23.4 km

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

## Day 0 False start (Twizel to Lake Pukaki return)

## Day 1 Mt Cook Village to Twizel

## Day 2 Lake Ohau Lodge to Omarama

## Day 3 Omarama to Kurow via Otematata

## Day 4 Kurow to Duntroon

## Day 5 Duntroon to Oamaru
