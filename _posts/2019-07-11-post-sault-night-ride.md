---
title: "A night ride through the Sault Lavender Fields, France 2019"
author: jaidev
categories:
  - albums
tags:
  - cycle
  - 19France
---

This post has been updated and should show a modified date if used in a layout.

Some text here


<link rel="stylesheet" href="https://unpkg.com/leaflet@1.5.1/dist/leaflet.css"
   integrity="sha512-xwE/Az9zrjBIphAcBb3F6JVqxf46+CDLwfLMHloNu6KEQCAWi6HcDUbeOfBIptF7tcCzusKFjFw2yuvEpDL9wQ=="
   crossorigin=""/>
   
   <!-- Make sure you put this AFTER Leaflet's CSS -->
<script src="https://unpkg.com/leaflet@1.5.1/dist/leaflet.js"
   integrity="sha512-GffPMF3RvMeYyc1LWMHtK8EbPv0iNZ8/oTtHPx9/cc2ILxQ+u905qIwdpULaqDkyBKgOaB57QTMg7ztg8Jm2Og=="
   crossorigin=""></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/leaflet-gpx/1.4.0/gpx.min.js"></script>

   
<div id="mapid" style="width: 600px; height: 400px;"></div>
<script>

var mymap = L.map('mapid').setView([44.093, 5.407], 13);

L.tileLayer('https://api.tiles.mapbox.com/v4/{id}/{z}/{x}/{y}.png?access_token=pk.eyJ1IjoibWFwYm94IiwiYSI6ImNpejY4NXVycTA2emYycXBndHRqcmZ3N3gifQ.rJcFIG214AriISLbB6B5aw', {
		maxZoom: 18,
		attribution: 'Map data &copy; <a href="https://www.openstreetmap.org/">OpenStreetMap</a> contributors, ' +
			'<a href="https://creativecommons.org/licenses/by-sa/2.0/">CC-BY-SA</a>, ' +
			'Imagery © <a href="https://www.mapbox.com/">Mapbox</a>',
		id: 'mapbox.streets'
	}).addTo(mymap);

var gpx = 'https://www.jdem.com.au/assets/2019-07-11-sault-night-ride/2019-07-11-sault-night-ride.gpx'; // URL to your GPX file or the GPX itself

new L.GPX(gpx, {async: true}).on('loaded', function(e) {
  map.fitBounds(e.target.getBounds());
}).addTo(map);

</script>

