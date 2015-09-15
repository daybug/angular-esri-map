# Change Log

All notable changes to this project will be documented in this file.
This project adheres to [Semantic Versioning](http://semver.org/).

[Upcoming changes][unreleased]

### Documentation

Examples pages are now driven by configurable JSON and have more consistent titles [#94](https://github.com/Esri/angular-esri-map/pull/94)

Using `ng-options` for zoom level select Set Center and Zoom example page so that it has the correct value selected initially [c8659fce](https://github.com/Esri/angular-esri-map/commit/c8659fce94a94c5361a4cb047410b7cf0c4c87e4)

### Enhancements
Geographic center coordinates are normalized prior to updating esriMap scope values. [#93](https://github.com/Esri/angular-esri-map/issues/93)

### Tests

Added functional testing using [Protractor](https://angular.github.io/protractor/#/) [#82](https://github.com/Esri/angular-esri-map/pull/82) [#94](https://github.com/Esri/angular-esri-map/pull/94)

### Maintenance

Published to NPM [#80](https://github.com/Esri/angular-esri-map/issues/80)

## [Beta 4][v1.0.0-beta.4]

### Added

* The esriMap directive's additional map options now support advanced options such as Extent and Popup. https://github.com/Esri/angular-esri-map/pull/71

### Changed

* The esriMap directive now reads additional map options by scope function binding, and these options are passed into the construction of a map from a webmapId. https://github.com/Esri/angular-esri-map/pull/71
* Changes to accommodate a thorough review of the map directive life cycle, and adjustments to make sure all properties are updated and events fired as expected. https://github.com/Esri/angular-esri-map/pull/76
* Several existing docs and test pages updated ([web map example](http://esri.github.io/angular-esri-map/#/examples/web-map) includes a legend).

### Fixed

* Additional Attributes Example Error: navigationMode must be 'css-transforms' or 'classic' [#65](https://github.com/Esri/angular-esri-map/issues/65)
* Load event now properly fires when using a web map. [#76](https://github.com/Esri/angular-esri-map/pull/76)

### New Demos

* [No Basemap](http://esri.github.io/angular-esri-map/#/examples/no-basemap) and [Additional Map Options](http://esri.github.io/angular-esri-map/#/examples/additional-map-options)

## [Beta 3][v0.0.1-beta.3]

### Added

* The esriLoader now takes a callback function to which it passes all loaded modules as arguments. https://github.com/Esri/angular-esri-map/pull/54
* Added support for a visible attribute on the esriFeatureLayer directive.
* Lazy loading of JSAPI and associated (minor) updates to esriLoader behavior. https://github.com/Esri/angular-esri-map/pull/60

### Changed

* Docs site uses JSAPI v.3.14 (#66) and Angular v1.4.4. https://github.com/Esri/angular-esri-map/pull/67

### Fixed

* Fixed script path (https://github.com/Esri/angular-esri-map/commit/6b4659c2d1d338ba752ddba8827f16fd12b4c330).

### New Demos

* [Deferred Map Example test page](http://esri.github.io/angular-esri-map/deferred-map.html)

Thank you to @willisd2, @ScottONeal, @thinking-aloud, and @jwasil for their contributions and continued patience.

## [Beta 2][v0.0.1-beta.2]

### Added

* The esriLoader factory can accept an array of module names and return an array of modules (thanks @trkbrkr2000). https://github.com/Esri/angular-esri-map/pull/45
* The esriMap directive can accept additional map options (thanks @eas604). https://github.com/Esri/angular-esri-map/pull/39
* Docs site includes formatted code snippets.

### Changed

* Docs site uses JSAPI v3.13.

### Fixed

* Dojo loader multipleDefine in docs (thanks @niblicroad). https://github.com/Esri/angular-esri-map/pull/38
* esrilegend.js was not found in gulp, renamed to esriLegend.js (thanks @eas604) https://github.com/Esri/angular-esri-map/pull/40

### New Demos

* [Registry Pattern](http://esri.github.io/angular-esri-map/#/examples/registry-pattern)
* [Additional Map Options](http://esri.github.io/angular-esri-map/#/examples/additional-attributes)
  * _NOTE: This demo page address has changed after Beta 3 to [Additional Map Options](http://esri.github.io/angular-esri-map/#/examples/additional-map-options)_

## [Beta 1][v0.0.1-beta.1]

### Added

* Initial public release.
* Includes directives for map, features layers, and legend and services to facilitate loading Esri modules and enabling controllers to reference the map object.

[unreleased]: https://github.com/Esri/angular-esri-map/compare/v1.0.0-beta.4...HEAD
[v1.0.0-beta.4]: https://github.com/Esri/angular-esri-map/compare/v0.0.1-beta.3...v1.0.0-beta.4
[v0.0.1-beta.3]: https://github.com/Esri/angular-esri-map/compare/v0.0.1-beta.2...v0.0.1-beta.3
[v0.0.1-beta.2]: https://github.com/Esri/angular-esri-map/compare/v0.0.1-beta.1...v0.0.1-beta.2
[v0.0.1-beta.1]: https://github.com/Esri/angular-esri-map/commits/v0.0.1-beta.1