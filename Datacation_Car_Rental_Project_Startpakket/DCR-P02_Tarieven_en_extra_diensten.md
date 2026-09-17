# Tarieven en extra diensten

Document-ID: DCR-P02
Versie: 1.0
Geldig vanaf: 2026-09-01
Herziening: 2026-12-01
Eigenaar: Verhuuradministratie
Taal: nl-NL
Tags: dagtarief, kilometers, extra bestuurder, prijsberekening

Fictieve bedrijfsregels voor de demonstratie. Geen echte verhuurovereenkomst.

## P02.1 Prijsbasis

Deze tariefkaart ondersteunt prijsvoorstellen en uitleg over bestaande boekingen. Alle huurprijzen zijn fictieve consumentenbedragen in euro, inclusief de in de demo aangenomen 21% btw. Zakelijke klanten hebben dezelfde prijzen. Borg en eigen risico staan apart en worden niet bij de huursom opgeteld.

De onderstaande tabel is een weergave van autos in datapakket 1.0. Gebruik bij bestaande boekingen altijd het daarin afgesproken dagtarief en de vastgelegde extra’s. Een nieuw catalogustarief verandert geen historische boeking.

## P02.2 Dagtarieven van de demovloot

| Auto | Model | Per dag | Borg | Eigen risico |
| --- | --- | --- | --- | --- |
| A001 | Toyota Aygo X | € 49 | € 500 | € 750 |
| A002 | Volkswagen Polo | € 59 | € 500 | € 750 |
| A003 | Renault Clio | € 55 | € 500 | € 750 |
| A004 | Toyota Corolla Touring Sports | € 85 | € 750 | € 1000 |
| A005 | Kia Niro EV | € 89 | € 750 | € 1000 |
| A006 | Volkswagen Golf | € 75 | € 750 | € 1000 |
| A007 | Opel Corsa | € 55 | € 500 | € 750 |
| A008 | Tesla Model 3 | € 109 | € 1000 | € 1500 |
| A009 | Peugeot 3008 | € 95 | € 750 | € 1000 |
| A010 | Skoda Octavia Combi | € 89 | € 750 | € 1000 |

## P02.3 Extra bestuurder

Een extra bestuurder kost € 10 per huurdag en moet vooraf worden geregistreerd en gecontroleerd. In dit datapakket is maximaal één extra bestuurder opgenomen. Andere extra’s, kortingen of beschermingspakketten zijn niet geprijsd; maak daarvoor geen bedrag op en leg een aanvraag aan de Manager Agent voor.

## P02.4 Huurprijs en kilometers berekenen

Huurdagen = het aantal begonnen perioden van 24 uur tussen ophalen en afgesproken inleveren, naar boven afgerond, met minimaal één dag. Huursom = huurdagen × (afgesproken dagtarief + extra’s per dag). Gebruik Europe/Amsterdam en de werkelijke tijdzoneoffset bij tijdsberekeningen.

Per huurdag zijn 200 kilometer inbegrepen. Meerprijs = het positieve verschil tussen gereden en inbegrepen kilometers × € 0,25. Bij minder gereden kilometers is de meerprijs € 0. Voor nacalculatie zijn de kilometerstanden bij uitgifte en retour nodig. De actuele km_stand van een auto alleen is onvoldoende. Ontbrekende standen betekenen onbekend, niet nul.

## P02.5 Brandstof en laden

Benzine- en hybrideauto’s worden met een volle tank uitgegeven en vol ingeleverd. Bij een elektrisch voertuig wordt het laadpercentage geregistreerd; het voertuig moet met minstens hetzelfde percentage terugkomen. Het uitgifterapport is leidend voor het gemeten niveau.

Kosten voor ontbrekende brandstof of lading moeten met een meetregistratie en kostenbewijs worden onderbouwd. Dit pakket bevat geen tarief voor bijtanken, laden of administratiekosten. De AI kan daarom geen dergelijke toeslag berekenen of toezeggen; een medewerker beoordeelt de afrekening.

## P02.6 Rekenvoorbeelden en antwoordgrenzen

DCR-1043: twee dagen × (€ 59 huur + € 10 extra bestuurder) = € 138. Er zijn 400 kilometer inbegrepen. De borg van € 500 is afzonderlijk en vormt geen onderdeel van deze € 138.

DCR-1055: drie dagen × (€ 109 + € 10) = € 357. DCR-1042: vier dagen × € 49 = € 196. Een voorstel voor één extra volle dag op dezelfde voorwaarden kost € 49; controleer eerst beschikbaarheid volgens DCR-P03.

Presenteer een uitkomst als prijsvoorstel zolang de wijziging niet is goedgekeurd en geregistreerd. Noem uitgangspunten, huurperiode, inbegrepen kilometers en borg afzonderlijk. Een ontbrekend gegeven of onverklaarde afwijking tussen tariefkaart en overeenkomst gaat naar de Manager Agent; pas het record niet stilzwijgend aan.
