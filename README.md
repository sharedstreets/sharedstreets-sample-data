# SharedStreets - Sample Data

This directory contains protocol buffer encoded SharedStreets sample data using the 2018-01-14 draft of the specification and preview release [v0.1.3](https://github.com/sharedstreets/sharedstreets-builder/releases/tag/0.1.2) of the [SharedStreets Builder](https://github.com/sharedstreets/sharedstreets-builder) application.

The files are named using spherical mercator [z-x-y] tile coordinates, and are encoded using [length delimited protobuf messages](https://developers.google.com/protocol-buffers/docs/techniques#streaming). Features that span a tile boundary are encoded in both tiles.

To convert PBF files to JSON, one can use [`sharedstreets-pbf`](https://github.com/sharedstreets/sharedstreets-pbf) to decode PBF to JSON using [Node.js](https://nodejs.org/en/) or directly from your Web browser.

## Sample Data URL

These sample data PBF files are hosted via GitHub pages:

**URL Pattern**

```
https://sharedstreets.github.io/sharedstreets-sample-data/{dataset}/{zoom}-{x}-{y}.{type}.pbf
```

**URL Example**

```
https://sharedstreets.github.io/sharedstreets-sample-data/nyc/11-602-769.geometry.pbf
```
