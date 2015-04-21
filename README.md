# map-marker-icons

Different marker icons for interactive mapping, e.g. for use with Leaflet or Google Maps.

Marker icons are simple PNG images. AI files are also included if you want to modify the markers.

Here is a simple usage of the icon for Leaflet:

    var blueHotelIcon = L.icon({
        iconUrl: 'https://github.com/christiankaiser/map-marker-icons/raw/master/icons/plain-blue-hotel.png',
        iconSize: [32, 41],
        iconAnchor:   [16, 40],
        popupAnchor:  [0, -40]
     });
    
    L.marker([46.18, 7.15], {icon: blueHotelIcon}).addTo(map).bindPopup('Sweet dreams hotel');

If you want to include the `leaflet-map-marker-icons.js` file into your code, you can create the same marker as follows:

	var blueHotelIcon = L.icon(mapMarkerIcons.plainBlueHotel);
	L.marker([46.18, 7.15], {icon: blueHotelIcon}).addTo(map).bindPopup('Sweet dreams hotel');

