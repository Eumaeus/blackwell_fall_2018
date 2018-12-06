# Places Instructions

Make a text file, named `places_your-last-name.txt`. Be sure it is *plain text* (make it in Atom (<https://atom.io>) or, if you use Word or GoogleDocs, be sure to save it as plain text.

You can download a [template file](https://github.com/Eumaeus/blackwell_fall_2018/blob/master/docs/places_template.txt) to get you started.

There are five "columns":

1. id
1. text-urn
1. placename
1. pleiadesUri
1. geojson

The first line of the text file should name those columns:

> `https://github.com/Eumaeus/blackwell_fall_2018/blob/master/docs/places_template.txt`

Each subsequent line is a record that must consist of the same number of columns, and the columns should be divided by the character `#`.

- The `id` column should contain a value, unique in your list: your last name, an "`_`" character, and a number, from 1 to however many entries you make.
- The `text-urn` column should identify the passage of text you are illustrating. The identifier should look like `urn:cts:greekLit:tlg0016.tlg001.eng.token:1.72.130`, where `1.72.130` is the place's name, in the passage of Herodotus, in English. **Make sure this is valid!** (see below)
- The `placename` column should contain the name of the place, as it appears in Herodotus, *e.g.* "Cyprus".
- The `pleiadesuri` column should contain a the complete URI-identifier from <https://pleiades.stoa.org>. It should look like this: `https://pleiades.stoa.org/places/707498` (for Cyprus).
- The `geojson` column is where you may, optionally, include data created at <http://geojson.io> defining an area. If the place is Sardis, a city, then you don't need this, since that is a point on a map. But if the place is an island, like Cyprus, or a region, you might choose to. If you do this, you have to make the multi-line geoJson data into a *single line*:

> {"type": "FeatureCollection", "features": [{"type": "Feature", "properties": {}, "geometry": {"type": "Polygon", "coordinates": [[[34.59045410156249, 35.71083783530009 ], [33.6016845703125, 35.36217605914681 ], [33.3270263671875, 35.348735749472546 ], [32.926025390625, 35.40696093270201 ], [32.9095458984375, 35.18278813800229 ], [32.6348876953125, 35.18727767598896 ], [32.530517578125, 35.137879119634185 ], [32.44262695312499, 35.06597313798418 ], [32.29431152343749, 35.097439809364204 ], [32.3162841796875, 34.92647493584645 ], [32.464599609375, 34.755153088189324 ], [32.7886962890625, 34.664840578219305 ], [32.882080078125, 34.646766246519114 ], [33.0084228515625, 34.56990638085636 ], [33.431396484375, 34.768691457552706 ], [33.607177734375, 34.8047829195724 ], [33.6566162109375, 34.985003130171066 ], [33.870849609375, 34.93548199355903 ], [34.07958984374999, 34.97150033361733 ], [33.892822265625, 35.18727767598896 ], [33.9422607421875, 35.31736632923788 ], [34.0521240234375, 35.31736632923788 ], [34.112548828125, 35.40696093270201 ], [34.32128906249999, 35.50092819950358 ], [34.5849609375, 35.68630240145625 ], [34.59045410156249, 35.71083783530009 ] ] ] } } ] }

**All of this must be on *one line*.**

So a comlete record for "Cyprus" will look like this:

> blackwell_1#urn:cts:greekLit:tlg0016.tlg001.eng.token:1.72.130#Cyprus#https://pleiades.stoa.org/places/707498#{"type": "FeatureCollection", "features": [{"type": "Feature", "properties": {}, "geometry": {"type": "Polygon", "coordinates": [[[34.59045410156249, 35.71083783530009 ], [33.6016845703125, 35.36217605914681 ], [33.3270263671875, 35.348735749472546 ], [32.926025390625, 35.40696093270201 ], [32.9095458984375, 35.18278813800229 ], [32.6348876953125, 35.18727767598896 ], [32.530517578125, 35.137879119634185 ], [32.44262695312499, 35.06597313798418 ], [32.29431152343749, 35.097439809364204 ], [32.3162841796875, 34.92647493584645 ], [32.464599609375, 34.755153088189324 ], [32.7886962890625, 34.664840578219305 ], [32.882080078125, 34.646766246519114 ], [33.0084228515625, 34.56990638085636 ], [33.431396484375, 34.768691457552706 ], [33.607177734375, 34.8047829195724 ], [33.6566162109375, 34.985003130171066 ], [33.870849609375, 34.93548199355903 ], [34.07958984374999, 34.97150033361733 ], [33.892822265625, 35.18727767598896 ], [33.9422607421875, 35.31736632923788 ], [34.0521240234375, 35.31736632923788 ], [34.112548828125, 35.40696093270201 ], [34.32128906249999, 35.50092819950358 ], [34.5849609375, 35.68630240145625 ], [34.59045410156249, 35.71083783530009 ] ] ] } } ] }

A complete record for "Sardis" would look like (note the final `#`; the data of the `geojson` column is optional, but you need to define the column):

> blackwell_2#blackwell_1#urn:cts:greekLit:tlg0016.tlg001.eng.token:1.7.30#Sardis#https://pleiades.stoa.org/places/550867#


## How to validate a URN

Go to <http://folio.furman.edu/herodotus.html> and paste a Herodotus URN into the URN field in the upper-left of the screen. Click "Retrieve Passage". If you see the passage of Herodotus, it is a valid URN. The web-app will tell you if it not valid. **This is the important thing to get right.**

