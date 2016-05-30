[![Build Status](https://travis-ci.org/wo-ist-markt/wo-ist-markt.github.io.svg?branch=master)](https://travis-ci.org/wo-ist-markt/wo-ist-markt.github.io)

# A map of farmer markets

A small visualization of the weekly markets in different cities. Available at: http://wo-ist-markt.de


## Data format

* The market data is stored in [GeoJSON format][geojson].
* The opening hours use the [OpenStreetMap opening hours format][osm-openinghours].
* Opening hours that cannot be expressed in that format can use the `opening_hours_unclassified`
  property (in that case, set the `opening_hours` property to `null`).


### Mandatory information

* Besides the actual market information map **coordinates** and **zoom level** must be provided.
  These information are being used to set the initial position of the map. They must be part of
  the city-specific GeoJSON file. Please adapt the format as being used in *cities/karlsruhe.json*.
* Further, the **data source** must be specified so it can be shown in the legend overlay.
* Finally add your city to the *cities/cities.json* file.


## Navigation

* The individual market data for supported cities is displayed when the city name is given in the
  address bar of the browser.

  Example: http://wo-ist-markt.de/#karlsruhe.

  By default or on error *Karlsruhe* is rendered.


## Supported cities

|City name|Data source|
|:---|:---|
|[Berlin][berlin-wikipedia]|[City of Berlin][berlin-markets]|
|[Bochum][bochum-wikipedia]|[City of Bochum][bochum-markets]|
|[Chemnitz][chemnitz-wikipedia]|[City of Chemnitz][chemnitz-markets]|
|[Dortmund][dortmund-wikipedia]|[City of Dortmund][dortmund-markets]|
|[Dresden][dresden-wikipedia]|[City of Dresden][dresden-markets]|
|[Duisburg][duisburg-wikipedia]|[Duisburg Kontor GmbH][duisburg-markets]|
|[Düsseldorf][duesseldorf-wikipedia]|[City of Düsseldorf][duesseldorf-markets]|
|[Erlangen][erlangen-wikipedia]|[City of Erlangen][erlangen-markets]|
|[Essen][essen-wikipedia]|[EVB][essen-markets]|
|[Karlsruhe][karlsruhe-wikipedia]|[City of Karlsruhe][karlsruhe-markets]|
|[Köln][koeln-wikipedia]|[City of Köln][koeln-markets]|
|[Leipzig][leipzig-wikipedia]|[City of Leipzig][leipzig-markets]|
|[Moers][moers-wikipedia]|[City of Moers][moers-markets]|
|[Mülheim an der Ruhr][muelheim-ad-ruhr-wikipedia]|[City of Mülheim an der Ruhr][muelheim-ad-ruhr-markets]|
|[München][muenchen-wikipedia]|[City of München][muenchen-markets]|
|[Münster][muenster-wikipedia]|[City of Münster][muenster-markets]|
|[Neu-Ulm][neu-ulm-wikipedia]|[City of Neu-Ulm][neu-ulm-markets]|
|[Paderborn][paderborn-wikipedia]|[City of Paderborn][paderborn-markets]|
|[Rostock][rostock-wikipedia]|[City of Rostock][rostock-markets]|
|[Schwerin][schwerin-wikipedia]|[City of Schwerin][schwerin-markets]|
|[Ulm][ulm-wikipedia]|[City of Ulm][ulm-markets]|
|[Witten][witten-wikipedia]|[Stadtmarketing Witten][witten-markets]|
|[Wuppertal][wuppertal-wikipedia]|[City of Wuppertal][wuppertal-markets]|



## Contributing

* Please make sure to read the [contributing guide](CONTRIBUTING.md).


## Development

Tests can be run using [npm][npm]:

    $ npm install  # Just once after you've cloned the repo

    $ npm test     # Whenever you want to run the tests


[geojson]: http://geojson.org
[osm-openinghours]: https://wiki.openstreetmap.org/wiki/Key:opening_hours/specification
[npm]: https://www.npmjs.com

[berlin-wikipedia]: https://en.wikipedia.org/wiki/Berlin
[berlin-markets]: http://daten.berlin.de/datensaetze/wochen-und-tr%C3%B6delm%C3%A4rkte
[bochum-wikipedia]: https://en.wikipedia.org/wiki/Bochum
[bochum-markets]: https://www.bochum.de/amt32/wochenmaerkte
[chemnitz-wikipedia]: https://en.wikipedia.org/wiki/Chemnitz
[chemnitz-markets]: http://chemnitz.de/chemnitz/de/aktuelles/ausschreibungen/marktausschreibung/index.html
[dortmund-wikipedia]: https://en.wikipedia.org/wiki/Dortmund
[dortmund-markets]: https://www.dortmund.de/de/leben_in_dortmund/stadtportraet/einkaufen/wochenmaerkte/
[dresden-wikipedia]: https://en.wikipedia.org/wiki/Dresden
[dresden-markets]: https://www.dresden.de/de/leben/sport-und-freizeit/maerkte-in-dresden.php
[duisburg-wikipedia]: https://en.wikipedia.org/wiki/Duisburg
[duisburg-markets]: https://www.duisburg.de/leben/maerkte_in_duisburg/index.php
[duesseldorf-wikipedia]: https://de.wikipedia.org/wiki/D%C3%BCsseldorf
[duesseldorf-markets]: https://www.duesseldorf.de/verbraucherschutz/marktverwaltung/wochen.shtml
[erlangen-wikipedia]: https://en.wikipedia.org/wiki/Erlangen
[erlangen-markets]: http://www.erlangen.de
[essen-wikipedia]: https://en.wikipedia.org/wiki/Essen
[essen-markets]: https://www.essen.de/rathaus/aemter/ordner_32/Wochenmaerkte.de.html
[koeln-wikipedia]: https://en.wikipedia.org/wiki/Cologne
[koeln-markets]: http://www.offenedaten-koeln.de/dataset/wochenmaerkte-koeln
[karlsruhe-wikipedia]: https://en.wikipedia.org/wiki/Karlsruhe
[karlsruhe-markets]: http://www.karlsruhe.de/b3/maerkte/wochenmarkte.de
[leipzig-wikipedia]: https://en.wikipedia.org/wiki/Leipzig
[leipzig-markets]: https://www.leipzig.de/freizeit-kultur-und-tourismus/einkaufen-und-ausgehen/maerkte/
[moers-wikipedia]: https://en.wikipedia.org/wiki/Moers
[moers-markets]: https://www.moers.de/de/stichwoerter/maerkte-7688193/
[muelheim-ad-ruhr-wikipedia]: https://en.wikipedia.org/wiki/Mülheim
[muelheim-ad-ruhr-markets]: https://www.muelheim-ruhr.de/cms/muelheimer_wochenmaerkte1.html
[muenchen-wikipedia]: https://en.wikipedia.org/wiki/M%C3%BCnchen
[muenchen-markets]: https://www.opengov-muenchen.de/dataset/maerkte
[muenster-wikipedia]: https://en.wikipedia.org/wiki/M%C3%BCnster
[muenster-markets]: http://www.muenster.de/stadt/maerkte/markt.html
[neu-ulm-wikipedia]: https://en.wikipedia.org/wiki/Neu-Ulm
[neu-ulm-markets]: http://nu.neu-ulm.de/de/neu-ulm-erleben/veranstaltungen/feste-maerkte/wochenmarkt/
[paderborn-wikipedia]: https://en.wikipedia.org/wiki/Paderborn
[paderborn-markets]: http://www.paderborn.de/microsite/wochenmarkt/marktinfos/109010100000079411.php?p=5,1
[rostock-wikipedia]: https://en.wikipedia.org/wiki/Rostock
[rostock-markets]: http://www.rostocker-wochenmaerkte.de/standorte-angebote/
[schwerin-wikipedia]: https://en.wikipedia.org/wiki/Schwerin
[schwerin-markets]: http://marketing.schwerin.info/stadtmarketing/aufgaben/Flaeche_Maerkte.html
[ulm-wikipedia]: https://en.wikipedia.org/wiki/Ulm
[ulm-markets]: http://www.ulm-messe.de/marktwesen/wochenmarkt_ulm_soeflingen.97943.21332,97940,97943.htm
[witten-wikipedia]:https://en.wikipedia.org/wiki/Witten
[witten-markets]:http://www.stadtmarketing-witten.de/einkaufen/wochenmaerkte.html
[wuppertal-wikipedia]:https://en.wikipedia.org/wiki/Wuppertal
[wuppertal-markets]:https://www.wuppertal.de/tourismus-freizeit/einkaufen/102370100000204430.php
