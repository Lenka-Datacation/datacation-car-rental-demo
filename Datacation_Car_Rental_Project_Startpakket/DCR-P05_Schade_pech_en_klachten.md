# Schade pech en klachten

Document-ID: DCR-P05
Versie: 1.0
Geldig vanaf: 2026-09-01
Herziening: 2026-12-01
Eigenaar: Operationeel manager
Taal: nl-NL
Tags: schade, pech, veiligheid, klacht

Fictieve bedrijfsregels voor de demonstratie. Geen echte verhuurovereenkomst.

## P05.1 Doel en voorrang

Deze procedure regelt meldingen over schade, storingen en klachten. Een nieuwe melding kan belangrijker zijn dan een oudere status zonder incident. De AI registreert wat de klant meldt als melding, zonder oorzaak, schuld of technische veiligheid vast te stellen.

Een melding over remmen, sturen, rook, brand, letsel of een onveilige positie krijgt direct de route SPOED_MENS. Wacht daarvoor niet op een klantmatch, volledig dossier of sentimentanalyse. Agent 1 kan deze voorrang al activeren. De operationeel medewerker neemt de behandeling over; overige analyses mogen alleen ondersteunend doorgaan.

## P05.2 Veiligheidsmelding afhandelen

Vraag alleen de gegevens die voor overdracht nodig zijn: locatie, bereikbaarheid, voertuig of boeking indien bekend en een korte omschrijving. Laat de medewerker direct passende hulp organiseren. De AI geeft geen reparatie-instructies, diagnose of toestemming om met een mogelijk onveilige auto door te rijden.

De agents markeren spoed direct in de achtergrond en pauzeren de normale afhandeling. De presentator onthult de melding met Next, net als de andere agentresultaten. Toon duidelijk dat dit een simulatie is: er wordt geen hulpdienst gebeld of medewerker buiten de demo gealarmeerd. Een werkelijk incident moet buiten deze demonstratie worden afgehandeld.

## P05.3 Schade zonder direct gevaar

Vraag wanneer en waar de schade is gezien, wat er is waargenomen en welk voertuig het betreft. De medewerker verzamelt het uitgifterapport, retourrapport, gedateerde foto’s, de klantverklaring en een gespecificeerde kostenonderbouwing. De dataset bevat deze bijlagen niet; de AI mag geen foto of handtekening verzinnen.

Een nieuwe schadeclaim, ontbrekend bewijs of betwiste toerekening gaat altijd naar een mens. De AI mag het eigen risico uit de overeenkomst toelichten, maar niet automatisch dat maximum in rekening brengen. Het bedrag eigen_risico_eur bewijst geen dekking, aansprakelijkheid of daadwerkelijke schadehoogte.

## P05.4 Klachten en sentiment

Een rustige vraag over een bekende status kan als routine worden behandeld. Lichte frustratie vraagt een begripvolle toon, maar is op zichzelf geen escalatie. Ernstige boosheid, een herhaald onopgelost contact of een dreiging met juridische stappen vereist menselijke beoordeling. Een rustig geformuleerde veiligheidsmelding blijft spoed.

Onderscheid onderbouwde contacthistorie van een klantclaim. Staat er “ik heb al drie keer gebeld”, noteer dan “klant meldt drie eerdere contacten” zolang de administratie dat niet bevestigt. De demo bevat geen volledige contacthistorie. Een klacht over een eerder dossier blokkeert niet automatisch een losstaande nieuwe huur.

## P05.5 Beoordeling en klantantwoord

De operationeel medewerker onderzoekt voertuig en incident; de financiële medewerker beoordeelt een betwiste inhouding of schadeafrekening. De Manager Agent verzamelt informatie en routeert, maar vervangt die menselijke bevoegdheid niet. Klachten krijgen als fictieve streeftermijn binnen één werkdag een eerste inhoudelijke update; beloof geen eindoplossing als onderzoek loopt.

Agent 6 benoemt het gemelde probleem, wat wel en niet bekend is en de volgende stap. Erken hinder zonder aansprakelijkheid of vergoeding toe te zeggen. “Ik heb uw melding ontvangen” mag; “wij hebben de remmen verkeerd gerepareerd” mag niet zonder vastgesteld onderzoek. Iedere uitgaande tekst krijgt menselijke review volgens DCR-P06.

## P05.6 Voorbeelden uit de dataset

DCR-1044: € 350 betwiste schade, uitgifterapport ontbreekt en schade is nog niet gefactureerd. Route MENS_BESLISSING met operationele beoordeling en financiële afhandeling. Geen automatische inhouding, kwijtschelding of terugbetaling voorstellen als definitief besluit.

DCR-1047 vermeldt op de peildatum geen defectmelding. Als Yusuf nu schrijft “de remmen werken niet goed”, ontstaat toch direct een nieuwe spoedmelding. Het ontbreken van een eerder geregistreerd defect is geen bewijs dat de huidige melding onjuist is.
