# Spaarplan-data

Dagelijkse gegevens voor de app Spaarplan: lopende aanbiedingen met ons eigen
kortingsoordeel, productgroepen, prijsreeksen, gerechten en supermarktfilialen.

- Prijsgeschiedenis: [Checkjebon](https://github.com/supermarkt/checkjebon) (MIT).
- Aanbiedingen: [PrijsProfeet](https://www.prijsprofeet.nl) (gratis laag, met naamsvermelding).
- Filialen: © OpenStreetMap-bijdragers, [ODbL](https://opendatacommons.org/licenses/odbl/).
- Oordelen, koppelingen en gerechten: eigen werk van Spaarplan.

`manifest.json` zegt wanneer de gegevens gebouwd zijn en welke bestanden erbij horen.
De app haalt het manifest op en daarna alleen de bestanden die veranderd zijn.

Drie pagina's horen bij de app en staan hier omdat de App Store er een openbaar adres
voor vraagt:

- [`PRIVACY.md`](PRIVACY.md) — wat de app wel en niet over het internet stuurt.
- [`ONDERSTEUNING.md`](ONDERSTEUNING.md) — waar je een probleem meldt en wat je dan
  kunt verwachten.
- [`METHODIEK.md`](METHODIEK.md) — hoe een kortingsoordeel tot stand komt, met de stand
  van vandaag erin. Deze pagina wordt bij elke ronde opnieuw gebouwd uit het scherm in
  de app zelf, zodat er nooit iets anders staat dan wat de app zegt.
