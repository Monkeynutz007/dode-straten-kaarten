# Dode Straten: kaarten

Kaarten voor **Dode Straten**, het zombiespel in je eigen gemeente. Elke kaart is een hele gemeente, in vakken
van 500 m, gemaakt uit open data door de kaartfabriek (GitHub Actions). Het spel laadt ze rechtstreeks van
GitHub Pages: niemand hoeft iets te installeren of te betalen.

- **Kaartenlijst:** [`kaarten.json`](https://monkeynutz007.github.io/dode-straten-kaarten/kaarten.json)
- **Je gemeente aanvragen:** [nieuwe aanvraag](https://github.com/Monkeynutz007/dode-straten-kaarten/issues/new?template=gemeente.yml).
  De fabriek kijkt elke 6 uur naar nieuwe aanvragen, maakt de kaart (een kwartier tot een uur) en laat het je
  weten. Elke kaart wordt ongeveer elke maand vernieuwd.

## Wat zit erin

| Bron | Wat | Licentie |
|---|---|---|
| OpenStreetMap | wegen, gebouwen, winkels, water, groen, hagen, straatmeubilair | ODbL, © OpenStreetMap-bijdragers |
| Overture Maps | gebouwen die niet in OSM staan, gemeten hoogtes | ODbL |
| Meta en World Resources Institute | echte bomen (plek en hoogte) | CC BY 4.0 |
| Copernicus Sentinel-2 | de echte kleur van velden, weides, bossen en heide | bevat aangepaste Copernicus Sentinel-gegevens |
| Mapillary | straatlantaarns, banken, borden, brandkranen, verkeerslichten | CC BY-SA 4.0 |
| Verkeersborden.Vlaanderen, Agentschap Wegen en Verkeer (alleen Vlaanderen) | de echte verkeersborden met hun bordcode | open data van AWV |
| Digitaal Vlaanderen (alleen Vlaanderen) | GRB-gebouwen en -percelen, wegvlakken, dakkleuren uit luchtfoto's, dakvormen uit LiDAR (DHMV II) | Modellicentie Gratis Hergebruik |

De kaarten zelf vallen onder de **ODbL** (Open Database License), net als OpenStreetMap.

## Hoe het werkt

De bestanden staan op de tak `gh-pages`: per gemeente een map met een `.vakken`-bestand, en `kaarten.json` met
de lijst. Bij elke update wordt die tak opnieuw geschreven als één commit, zodat deze repository niet groeit.
