# @turf/truncate

# truncate

Takes a GeoJSON Feature or FeatureCollection and truncates the precision of the geometry.

**Parameters**

-   `layer` **([Feature](http://geojson.org/geojson-spec.html#feature-objects) \| [FeatureCollection](http://geojson.org/geojson-spec.html#feature-collection-objects))** any GeoJSON Feature or FeatureCollection
-   `precision` **\[[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)]** coordinate decimal precision (optional, default `6`)
-   `coordinates` **\[[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)]** maximum number of coordinates (primarly used to remove z coordinates) (optional, default `2`)

**Examples**

```javascript
var point = {
    "type": "Feature",
    "geometry": {
        "type": "Point",
        "coordinates": [
            70.46923055566859,
            58.11088890802906,
            1508
        ]
    },
    "properties": {}
};
var pointTrunc = turf.truncate(point);
//= pointTrunc
```

Returns **([Feature](http://geojson.org/geojson-spec.html#feature-objects) \| [FeatureCollection](http://geojson.org/geojson-spec.html#feature-collection-objects))** layer with truncated geometry

<!-- This file is automatically generated. Please don't edit it directly:
if you find an error, edit the source file (likely index.js), and re-run
./scripts/generate-readmes in the turf project. -->

---

This module is part of the [Turfjs project](http://turfjs.org/), an open source
module collection dedicated to geographic algorithms. It is maintained in the
[Turfjs/turf](https://github.com/Turfjs/turf) repository, where you can create
PRs and issues.

### Installation

Install this module individually:

```sh
$ npm install @turf/truncate
```

Or install the Turf module that includes it as a function:

```sh
$ npm install @turf/turf
```
