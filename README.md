# Spaarplan-data

Openbare pagina's bij de app Spaarplan, en het manifest van de dagelijkse gegevens.

De gegevens zelf staan hier sinds 30 september 2026 niet meer: de app haalt ze bij onze
eigen server. De aanbiedingen komen van [PrijsProfeet](https://www.prijsprofeet.nl), en
hun voorwaarden staan niet toe dat hun gegevens in een openbare repository staan.

`manifest.json` zegt wanneer de laatste set gegevens gebouwd is, hoeveel aanbiedingen erin
zitten en welke bestanden erbij horen (grootte en sha256). Er staan geen gegevens in.

Drie pagina's horen bij de app en staan hier omdat de App Store er een openbaar adres
voor vraagt:

- [`PRIVACY.md`](PRIVACY.md) — wat de app wel en niet over het internet stuurt.
- [`ONDERSTEUNING.md`](ONDERSTEUNING.md) — waar je een probleem meldt en wat je dan
  kunt verwachten.
- [`METHODIEK.md`](METHODIEK.md) — hoe een kortingsoordeel tot stand komt, met de stand
  van vandaag erin. Deze pagina wordt bij elke ronde opnieuw gebouwd uit het scherm in
  de app zelf, zodat er nooit iets anders staat dan wat de app zegt.
