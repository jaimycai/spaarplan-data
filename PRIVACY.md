# Privacy — Spaarplan

*Bijgewerkt op 21 oktober 2026. Dit is dezelfde tekst als het scherm Privacy in de app,
geschreven voor een openbare pagina omdat de App Store daar een adres voor vraagt.*

## Het korte antwoord

Spaarplan verzamelt niets over jou. Er is geen account, geen inlog, geen advertentie, geen
analytics en geen enkele vorm van tracking. De maker van deze app ontvangt geen gegevens
over jou. Er is één server van hem, en die geeft de app alleen de verse prijzen; hij
krijgt niets over jou mee en houdt niets bij.

Wat je in de app doet, staat op je eigen toestel en verdwijnt als je de app verwijdert: je
boodschappenlijst, welke supermarkten je koos, je dieet en allergenen, je thema, de
producten en woorden die je in de gaten houdt, wat er bij In huis staat en de wekkers van de
kookstand. Dat geldt ook voor de nummers van je
klantenkaarten: de app tekent de streepjescode zelf, en het nummer staat alleen op je toestel.
Staat de reservekopie van je iPhone aan
(iCloud of je computer), dan gaat dit mee in die reservekopie, net als bij je andere apps; die
is van jou en van Apple, en wij kunnen er niet bij. Scan je een kaart of een product in de
winkel, dan vraagt de app om je camera; die leest alleen de streepjescode en bewaart geen foto.

Je eigen recepten staan ook alleen op je toestel, met de foto's die je erbij zet. Maak je zelf
een foto van een gerecht bij een eigen recept, dan vraagt de app ook om je camera. Kies je
liever een foto uit je foto's, dan krijgt de app alleen de foto die je kiest en niet de rest.
Zo'n foto blijft op je toestel en gaat nergens heen.

## Wat er wél over het internet gaat

Vijf dingen, en geen daarvan zegt iets over wie je bent.

**Productfoto's.** Die zitten niet in de app maar staan bij de supermarkten zelf. Je
telefoon haalt ze rechtstreeks op bij hun beeldservers. Die ketens zien daardoor dat er
een verzoek om een plaatje binnenkomt, zoals bij elke website die een foto toont. Wij zien
dat verzoek niet.

**Het verversen van de prijsgegevens.** Bij het starten kijkt de app hoogstens één keer
per uur of er nieuwe gegevens zijn. Dat is één klein bestand bij onze eigen server,
een Worker bij Cloudflare, zonder parameters, en met een vaste sleutel die in elke kopie
van de app dezelfde is. Zijn de gegevens veranderd, dan haalt de app alleen de veranderde
bestanden op. Cloudflare ziet daarbij het IP-adres van je telefoon, zoals elke server dat
ziet die een antwoord terugstuurt. Wij bewaren het niet: die server houdt geen logboek,
geen IP-adres en geen teller per toestel bij. De enige uitzondering is het schrijven van een
recept (hieronder): daar telt hij een minuut lang hoe vaak een IP-adres het vroeg, tegen
misbruik, en daarna niet meer.

**Een postcode opzoeken.** Alleen als je er zelf een intikt. Die gaat één keer naar de
Locatieserver van PDOK, een dienst van het Kadaster, zonder account en zonder sleutel. Wij
bewaren daarna één punt op je toestel, afgerond op ongeveer tien meter, zonder
geschiedenis.

**De knop naar de winkel op een productscherm.** Alleen als je erop tikt. Bij de meeste
ketens heet hij "Bekijk bij ..." en opent hij de productpagina zelf; het adres komt uit onze
bron en wordt kaal gemaakt — geen parameters, geen herkenning, geen verwijzing naar ons.

Levert onze bron voor dat product geen productpagina, dan heet de knop "Zoek bij ..." en gaat
hij naar de zoekpagina van die winkel met de productnaam erin. DekaMarkt en Hoogvliet hebben
geen zoekadres dat je kunt delen; daar zet de knop de productnaam op je klembord en opent hij
hun voorpagina, zodat je hem zelf in hun zoekbalk kunt plakken. Dat klembord is van jou: wij
lezen het niet en wij weten niet wat je ermee doet. De folders in Zoeken openen op dezelfde
manier de folder op de site van de winkel.

Ook dan bezoek jij die site zelf en sturen wij niets mee.

**Een recept importeren.** Alleen als je zelf een adres plakt of deelt. Een link van een
receptsite haalt je telefoon zelf op, net zoals je browser dat zou doen; bij Pinterest de pin en
daarna de receptsite waar die naar wijst. Weigert een site de app, dan haalt onze server die ene
pagina op (alleen als er een recept op staat), en lukt ook dat niet, dan opent je telefoon de
pagina onzichtbaar in een webweergave, zoals Safari. De site kan daarbij zijn eigen scripts en
cookies gebruiken; die worden niet bewaard.

Een link van TikTok of YouTube gaat naar onze eigen server (sinds 19-10-2026). Die vraagt bij
TikTok de video op, en bij YouTube de titel en de beschrijving via de YouTube API Services van
Google. Daarvoor gelden de voorwaarden van YouTube (https://www.youtube.com/t/terms) en de
privacyverklaring van Google (https://policies.google.com/privacy). Onze server bewaart wat het
platform over die link zegt een week, zodat dezelfde link niet steeds opnieuw wordt opgevraagd.
Wie de link deelde, bewaart hij niet.

Een post van TikTok, Instagram of Facebook opent je telefoon ook zelf, onzichtbaar in een
webweergave, zoals Safari dat doet (sinds versie 1.3.0). Zo leest hij de tekst bij de post, de
omslagfoto en bij TikTok de automatische ondertitels. Het platform kan daarbij zijn eigen scripts
en cookies gebruiken; die worden niet bewaard.

Staat het recept niet of maar half in de tekst bij de video, dan vult onze server het aan.
Daarvoor gaan de naam van het gerecht (die leest de app af, of hij vraagt hem aan jou) en de
tekst en ondertitels die wel bij de video stonden naar onze server. Die schrijft er een recept
bij met een taalmodel van Cloudflare (Workers AI). Heeft dat model het te druk, dan gaat dezelfde
vraag naar een taalmodel van Groq, een bedrijf in de Verenigde Staten
(https://groq.com/privacy-policy), dat niet traint op wat wij sturen. Lukt ook dat niet, dan
schrijft het taalmodel van Apple het recept op je telefoon zelf. Onze server bewaart een recept
een maand bij die naam en tekst, zodat dezelfde vraag niet opnieuw naar een model gaat. Wie het
vroeg, bewaart hij niet. In de app staat zo'n recept als "Aangevuld door Spaarplan".

Heeft een recept geen foto, dan gaat alleen de naam van het gerecht naar onze server. Staat dat
gerecht in onze fotocatalogus, dan haalt je telefoon die foto daar op, met "Beeld gemaakt door
Spaarplan" erop.

Het recept uit de video zelf haal je binnen met een schermafbeelding. Die leest je telefoon zelf
(met de tekstherkenning van iOS), en de afbeelding gaat nergens heen. Wat eruit komt blijft op je
toestel.

## Je locatie

De app vraagt alleen toestemming als je op "gebruik mijn locatie" tikt, en alleen voor
gebruik terwijl de app open is. Er is geen achtergrondlocatie. Je positie gaat nergens
heen: hij wordt op je toestel gebruikt om te bepalen welke filialen binnen de straal
vallen die jij koos.

Wil je dat niet, dan typ je een postcode. Wil je ook dat niet, dan werkt de app verder
gewoon — je ziet alleen geen afstanden.

## Meldingen

De app stuurt geen pushberichten. Er is geen pushdienst, geen token en geen server van ons die
berichten stuurt;
technisch kán deze app je geen bericht sturen.

Wat er wél is, en alleen als je het zelf aanzet (bij Ik voor een product dat je bewaakt, of
op Zoeken door een woord te volgen): je telefoon haalt hoogstens één keer per twaalf uur
dezelfde bestanden op als bij het starten, kijkt zélf of daar een product tussen
zit dat jij bewaakt, of een aanbieding met ons oordeel Echt voordeel bij een woord dat je
volgt, en maakt de melding op het toestel. Wij weten niet welke producten of woorden je
volgt en wij weten niet dat je een melding kreeg.

Het is geen prijsalarm dat op de minuut werkt: iOS bepaalt zelf wanneer een achtergrondtaak
draait, en forceer je de app af, dan stopt die taak tot je hem weer opent.

Zet je in de kookstand een wekker, dan plant je telefoon zelf een melding in voor het moment
dat de tijd om is. Mocht de app nog geen meldingen geven, dan vraagt hij dat eerst. Inspreken
bij In huis gaat met de microfoon van het toetsenbord van iOS: de app vraagt zelf geen toegang
tot je microfoon.

## Waar de gegevens vandaan komen

- **Prijsgeschiedenis:** Checkjebon, een open databestand onder de MIT-licentie dat sinds
  november 2022 dagelijks prijslijsten vastlegt.
- **Aanbiedingen:** PrijsProfeet.
- **Filialen en openingstijden:** OpenStreetMap-bijdragers, onder de ODbL.

De supermarkten zijn geen partner van deze app. Hun merknamen en productfoto's worden
gebruikt om producten te herkennen en te benoemen. Er is geen samenwerking en er wordt
niets betaald, in geen van beide richtingen.

## Kinderen

De app is niet op kinderen gericht en vraagt van niemand persoonsgegevens, ook niet van
kinderen.

## Vragen

Stel ze via de ondersteuningspagina die bij deze app in de App Store staat.
