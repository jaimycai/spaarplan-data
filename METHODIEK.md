# Hoe wij prijzen meten

*Deze pagina is op 22 september 2026 gemaakt uit het scherm Hoe wij prijzen meten in de app Spaarplan, en zegt dus letterlijk hetzelfde. De getallen zijn geteld in de gegevens waar de app zelf mee draait.*

Deze app beweert niet dat iets goedkoop is — dat beweert elke folder. Hij laat zien wat wij zelf gemeten hebben en trekt daar één conclusie uit. Hieronder staat hoe die conclusie tot stand komt, welke regels erachter zitten, en wat wij niet kunnen zien.

## Waar de prijzen vandaan komen

Wij werken met twee lagen. De prijsgeschiedenis komt uit Checkjebon, een openbaar databestand onder de MIT-licentie dat sinds november 2022 dagelijks de prijslijsten van Nederlandse supermarkten vastlegt. Wij lezen die geschiedenis dag voor dag uit en bouwen er per product een eigen reeks van: welke prijs gold wanneer, en op hoeveel dagen hebben wij die prijs werkelijk gezien. In deze versie van de app loopt die reeks tot en met 21 september 2026.

Wat er op dit moment in de aanbieding is, komt uit PrijsProfeet. Die twee lagen doen verschillend werk: PrijsProfeet zegt wat nu een aanbieding heet, onze eigen reeks zegt of die aanbieding ook een verlaging is.

Onze reeks heeft gaten. Er zijn kalenderdagen waarop er niets binnenkwam, en die dagen tellen wij niet mee als meting. Waar het uitmaakt zetten wij erbij hoeveel meetdagen wij misten, want vierhonderd metingen en vierhonderd dagen zijn niet dezelfde uitspraak.

## Waar de winkels vandaan komen

De filialen op het scherm In de buurt komen uit OpenStreetMap (© OpenStreetMap- bijdragers, ODbL): plek, adres en, waar OpenStreetMap ze heeft, openingstijden. Dat is een aparte tabel naast onze prijsdata. Onze prijzen zijn webshopprijzen per keten. Wat een product in een bepaald filiaal kost weten wij niet, en dat zetten wij dus nergens neer. De afstand is hemelsbreed, vanaf de plek of postcode die je zelf koos.

## Waar de zin 'Waarom deze week' vandaan komt

Bij elk gerecht staat per winkel een eigen zin die zegt waarom het deze week een goede keuze is, en je ziet de zin van de winkel die op datzelfde scherm staat. Die zin schrijft een taalmodel, op basis van precies de cijfers die wij bij díé winkel maten: de prijs per portie met en zonder actie, en welke ingrediënten daar in de aanbieding zijn. Daarna keurt code de zin: elk getal erin moet in die cijfers voorkomen, een andere keten mag niet genoemd worden en gezondheidsclaims en beschuldigingen zijn verboden. Een zin die daar niet doorheen komt, verdwijnt. Dan staat er liever niets. Het model kiest woorden, nooit getallen.

## Elke ochtend om 08:15 opnieuw

De gegevens in deze app zijn geen momentopname die wij ooit een keer gemaakt hebben. Elke ochtend om kwart over acht halen wij de nieuwe dag op, bouwen wij de prijsreeksen opnieuw, vragen wij de lopende aanbiedingen op en berekenen wij elk oordeel opnieuw. Kwart over acht is ná de dagelijkse commit van Checkjebon, die tussen half zeven en half acht komt. De stand die je nu voor je hebt komt uit de ronde van 22 september 2026.

Die ronde publiceert alles of niets. Er wordt gebouwd in een aparte map, en pas als alle controles gehaald zijn wordt die map in één keer omgewisseld: de databestanden zijn nooit half nieuw. Zakt het aantal aanbiedingen te hard, mist een gerecht zijn prijs of ziet een databestand er beschadigd uit, dan gaat de ronde niet door en blijft de stand van de vorige nacht staan.

Dat is een bewuste keuze, en het is de reden dat er soms een dag tussen zit: een oudere waarheid is beter dan een verse onwaarheid. De datum waarop wij voor het laatst gebouwd hebben staat onderaan deze pagina, zodat je het zelf kunt zien.

## De stand van vandaag

Zo ziet dit bestand er nu uit: 10.933 aanbiedingen die vandaag nog lopen, naast een prijsgeschiedenis die tot en met 21 september 2026 loopt. Aanbiedingen waarvan de einddatum voorbij is tellen wij hier niet mee, net zomin als op Vandaag. Elke aanbieding krijgt precies één oordeel.

De eerste drie zijn een oordeel over de verlaging. Bij vers zetten wij onze meting er wel naast maar spreken wij dat oordeel niet uit, en bij de laatste zeggen wij helemaal niets. Hoe groot dat laatste deel is, staat hieronder.

| Oordeel | Aantal | Aandeel |
|---|---:|---:|
| Echt voordeel | 5.385 | 49% |
| Eerder al zo goedkoop | 52 | 0,5% |
| Geen verlaging in de webshopprijs | 266 | 2% |
| Vers: wij geven geen oordeel over de korting | 997 | 9% |
| Te weinig gegevens | 4.233 | 39% |

## Wat "te weinig gegevens" betekent

Een aanbieding krijgt dat label als wij er geen eigen prijsreeks bij hebben waaruit wij een referentieprijs kunnen halen. Dat gebeurt op twee manieren. Óf wij vinden het product niet terug in onze prijsgeschiedenis — de aanbiedingenbron en de prijsgeschiedenis schrijven productnamen niet hetzelfde op, en wij koppelen alleen wat wij zeker weten. Óf wij vinden het wel terug, maar volgden het te kort of te onregelmatig om over dertig dagen iets te kunnen zeggen.

Dat is geen randgeval. Het overkomt vandaag 4.233 van de 10.933 aanbiedingen: 39%. Bij geen enkele daarvan staat een referentieprijs in onze gegevens, dus er valt ook niets te tonen — geen bedrag, geen percentage, geen grafiek met een stippellijn.

Wij tonen die aanbiedingen wél. Ze staan in Zoeken en je kunt ze op je lijst zetten, met het bedrag dat de winkel noemt erbij. Wat er niet bij staat is een oordeel van ons, want dat hebben wij niet. Zo een aanbieding kan uitstekend zijn. Wij weten het alleen niet, en dat is iets anders dan dat hij niets voorstelt.

Bij hele winkels kan dat zo zijn. Van ALDI en Ekoplaza draagt vandaag geen enkele aanbieding een oordeel: wij hebben er bij geen van die producten een referentieprijs bij die wij zelf gemeten hebben. Dat staat ook bij Mijn winkels, met de aantallen erbij. Kun je zo een winkel daar aanvinken, dan zie je het dus voordat je dat doet. Winkels waarvan onze prijsbron helemaal stilviel staan er apart en zijn niet te kiezen.

## Wij meten webshopprijzen, geen schapprijzen

Alles wat wij tonen komt uit de online winkels van de ketens. Een supermarkt mag in het filiaal een andere prijs voeren dan op de website, en veel acties gelden alleen in de winkel of alleen in een regio. Die zien wij niet.

Wijkt de prijs in het schap af van wat hier staat, dan heeft het schap gelijk. Wij zijn een tweede meting, geen kassa.

## De vijf oordelen

Elk product dat wij tonen krijgt precies één van deze vijf. Ze staan er niet om een winkel te beoordelen maar om te zeggen wat onze eigen reeks laat zien.

**Echt voordeel** — De prijs van vandaag ligt onder de laagste prijs die wij in de dertig dagen daarvoor bij die keten maten. Het bedrag en het percentage rekenen wij op die laagste eerdere prijs, en wij zetten erbij hoe vaak wij in die periode gemeten hebben.

**Eerder al zo goedkoop** — De prijs van vandaag ligt wel onder de laagste prijs die wij in de dertig dagen daarvoor bij die keten maten, maar minder dan tien cent of minder dan vijf procent eronder. Zo een verschil noemen wij geen verlaging, en wij rekenen er dus ook geen bedrag of percentage op.

**Geen verlaging in de webshopprijs** — Wij zagen de webshopprijs niet dalen. Dit is een meting en geen oordeel over de aanbieding: de winkel kan er een voordeel in zien dat in de webshopprijs geen spoor nalaat. Is er een voorwaarde zoals 1 + 1 gratis, dan zetten wij die erbij en rekent ons percentage op de stuksprijs die daarbij hoort.

**Vers: wij geven geen oordeel over de korting** — Bij verse producten schrijft de wet geen referentie van dertig dagen voor, en wij doen over de verlaging dan ook geen uitspraak. Wij zetten er alleen onze eigen meting naast: de laagste prijs die wij in diezelfde dertig dagen bij die keten maten, met het aantal dagen waarop wij toen gemeten hebben.

**Te weinig gegevens** — Wij hebben dit product te kort of te onregelmatig gemeten om er iets over te zeggen. Dan zeggen wij niets. Dat overkomt een groot deel van de catalogus, en dat is de bedoeling.

## De dertig dagen komen uit de wet

Wie een prijsverlaging aankondigt, moet daarbij de laagste prijs vermelden die hij in de dertig dagen vóór die verlaging hanteerde. Dat staat in artikel 5a van het Besluit prijsaanduiding producten, de Nederlandse uitwerking van de Europese Omnibusrichtlijn. De regel bestaat omdat een prijs die eerst kort omhoog gaat en daarna met veel vertoon weer zakt, anders als korting zou tellen.

Wij hanteren hetzelfde venster van dertig dagen, maar met onze eigen metingen als bron. Wij toetsen daarmee niet of een winkel zich aan die regel houdt — wij weten niet welke prijs hij in zijn eigen administratie als referentie voert. Wij zeggen alleen wat wij in die dertig dagen zelf gezien hebben.

## Waarom verse producten daarbuiten vallen

Datzelfde artikel maakt een uitzondering voor producten die snel bederven of maar kort houdbaar zijn: groente, fruit, vlees, vis, zuivel en brood. Een referentie van dertig dagen slaat daar nergens op, want de partij van vandaag is niet de partij van vorige maand en de prijs beweegt met het seizoen en de oogst mee.

Bij zulke producten laten wij het oordeel over de verlaging weg en zetten wij onze eigen meting uit diezelfde dertig dagen ernaast. Welke producten dat zijn leiden wij af uit de categorie die de bron meegeeft en uit woorden in de productnaam. Er is geen twijfelpad: één treffer is genoeg. Dat gaat dus ook mis. Een douchegel of een allesreiniger met het woord yoghurt of bloemen in de naam krijgt zo het label vers, terwijl daar niets aan bederft.

## Het percentage rekenen wij op de referentieprijs

Een korting kun je op twee manieren uitrekenen: op de prijs van gisteren of op de laagste prijs uit de dertig dagen ervoor. Het Hof van Justitie van de Europese Unie besliste in de zaak C-330/23 (Aldi Süd) dat het die laatste moet zijn. Anders zou een winkel de prijs eerst kunnen verhogen en daarna een korting kunnen berekenen op een bedrag dat bijna niemand betaald heeft.

Wij doen het net zo. Kost een product vandaag € 1,50 en was het gisteren € 2,00, maar maten wij binnen die dertig dagen ook € 1,60, dan is € 1,60 onze referentie en rekenen wij het percentage daarop. Dat levert een lager, maar eerlijker getal op.

## Wat wij niet zien

Wat een bulkactie kost als je er maar één meeneemt. Onze bron geeft de stuksprijs zoals hij ónder de actie geldt: bij 1 + 1 gratis is dat de prijs per stuk als je er twee pakt. Wij rekenen ons percentage op dat bedrag en zetten de voorwaarde erbij, op de kaart, op je lijst en bij het product. Wat één stuk los kost staat er niet in, dus dat zeggen wij ook niet.

Ledenprijzen. Kortingen die alleen gelden met Bonuskaart, Lidl Plus of Jumbo Extra's staan niet in onze bron. Wij tonen ze niet, ook niet als schatting.

De prijs in de winkel zelf. Zie hierboven: wij meten webshops. Wat er op het schapkaartje staat, in welk filiaal dan ook, is voor ons onzichtbaar.

## Wat wij met opzet weglaten

Alcohol, tabak en zuigelingenvoeding komen niet op Vandaag en niet bij Koken, ook niet als wij er een verlaging van maten; dat zijn er vandaag 900 van de 10.933. Voor zuigelingenvoeding is dat de wet: het Warenwetbesluit Zuigelingenvoeding verbiedt prijsacties. Voor alcohol en tabak is het onze eigen keuze — een app die kortingen aanprijst hoort dat met deze producten niet te doen. Zoeken vindt ze wel, want iets onvindbaar maken is geen eerlijkheid.

## Wij zeggen liever niets dan iets onjuists.

Daarom staat er bij een groot deel van de producten dat wij te weinig gemeten hebben, is de feed soms dun, en vullen wij een gat in onze reeks nooit op met een schatting.

---

Prijsgeschiedenis: Checkjebon (MIT, open data), door ons gemeten tot en met 21 september 2026. Aanbiedingen: PrijsProfeet. Deze gegevens zijn gebouwd op 22 september 2026 en worden elke ochtend om 08:15 opnieuw gebouwd.
