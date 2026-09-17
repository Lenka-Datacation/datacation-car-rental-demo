# Wijzigen verlengen en annuleren

Document-ID: DCR-P03
Versie: 1.0
Geldig vanaf: 2026-09-01
Herziening: 2026-12-01
Eigenaar: Verhuuroperatie
Taal: nl-NL
Tags: wijzigen, verlengen, annuleren, beschikbaarheid

Fictieve bedrijfsregels voor de demonstratie. Geen echte verhuurovereenkomst.

## P03.1 Beoordeling van een wijziging

Deze procedure bepaalt wanneer een wijziging of annulering als standaardgeval kan worden voorbereid. Controleer eerst de juiste boeking, de klantrol, de huidige status en het gewenste nieuwe tijdvak. De oorspronkelijke afspraak blijft gelden totdat de wijziging is bevestigd.

Voor een nog niet begonnen huur mag Agent 5 een datumwijziging zonder aparte wijzigingskosten voorstellen als dezelfde auto beschikbaar is en de overige voorwaarden gelijk blijven. Bereken de nieuwe huurduur tegen het afgesproken dagtarief plus extra’s. Een andere auto of vestiging, een tariefuitzondering of een terugbetaling vraagt een medewerker volgens DCR-P06.

## P03.2 Beschikbaarheid vaststellen

Blokkeer voor iedere niet-geannuleerde boeking de periode van ophalen tot twee uur na inleveren. Een aanvraag mag geen andere blokkade overlappen. Sluit bij een wijziging de eigen bestaande boeking uit van die vergelijking, maar controleer alle overige boekingen, ook van dezelfde klant.

Een optie blokkeert tot de expliciete vervaltijd; de geboekte huurperiode blijft daarvoor het gereserveerde tijdvak. Onderhoud blokkeert inzet zolang de gereedmelding ontbreekt. Als onderhoud vóór een toekomstige huur gepland eindigt, mag de AI die planning noemen, maar geen definitieve inzetbaarheid garanderen.

## P03.3 Lopende huur verlengen

Een verlenging moet vóór de afgesproken inlevering worden aangevraagd. Tot en met twee extra huurdagen van elk 24 uur mag Agent 5 een routinevoorstel maken als beschikbaarheid, huurbetaling en borg in orde zijn en geen incident of geschil speelt. Bereken de extra begonnen 24-uursperioden tegen dezelfde dagprijs en extra’s.

Meer dan twee extra huurdagen, een aanvraag na de inlevertijd, een planningconflict of een ontbrekende gereedmelding gaat naar de Manager Agent. De klant moet akkoord gaan met de aanvullende prijs; een medewerker registreert de wijziging en eventuele betaling. Een mondelinge wens is geen verlengde huur.

## P03.4 Annulering voor aanvang

Bij ontvangst minimaal 24 uur vóór ophalen zijn de annuleringskosten € 0. Minder dan 24 uur vóór ophalen zijn de kosten één afgesproken huurdag inclusief de geboekte extra’s, maximaal de totale huursom. Exact 24 uur valt dus onder kosteloos annuleren. Een optie kan vóór bevestiging kosteloos vervallen of worden ingetrokken.

Te restitueren huur = het hoogste van € 0 en (betaald_eur − terugbetaald_eur − annuleringskosten). Nooit meer terugbetalen dan het nog aanwezige huurtegoed. Een te innen restbedrag, no-show, annulering na aanvang of afwijkende afspraak vereist menselijke beoordeling. De borg wordt afzonderlijk behandeld volgens DCR-P04.

## P03.5 Uitvoering en communicatie

Agent 5 berekent uitsluitend het voorstel en vermeldt de gebruikte ontvangsttijd. Agent 6 schrijft “wij kunnen dit voor u aanvragen” zolang uitvoering niet is bevestigd. Iedere daadwerkelijke annulering, financiële mutatie of wijziging in deze demo wacht op een menselijke beslissing; uitgaande berichten blijven concepten tot review.

Bij een al geannuleerde boeking wordt geen tweede annulering of terugbetaling aangemaakt. Controleer de bestaande terugbetaling en verwijs daarnaar. Geef geen gegarandeerde bankdatum.

## P03.6 Voorbeelden uit de dataset

DCR-1042 eindigt 18 september om 10:00. Een verzoek om terugbrengen op 19 september om 10:00 levert één extra dag van € 49 op. Er is in de vaste dataset geen opvolgende boeking op A001; na de overige controles kan dit een routinevoorstel worden.

DCR-1043 eindigt 17 september om 10:00. Verlengen tot 18 september om 10:00 botst met de twee uur voorbereiding vóór DCR-1053, die diezelfde ochtend begint. Het systeem mag dit niet automatisch goedkeuren, ook al zijn beide boekingen van Daan van Dijk.

DCR-1050 is op 15 september geannuleerd voor ophalen op 23 september. De volledige € 285 is al terugbetaald. Het nog te restitueren bedrag is € 0.
