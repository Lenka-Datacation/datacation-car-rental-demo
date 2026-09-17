# Escalatie bevoegdheden en agentoverdracht

Document-ID: DCR-P06
Versie: 1.0
Geldig vanaf: 2026-09-01
Herziening: 2026-12-01
Eigenaar: Demo proceseigenaar
Taal: nl-NL
Tags: routering, escalatie, menselijke review, bevoegdheden

Fictieve bedrijfsregels voor de demonstratie. Geen echte verhuurovereenkomst.

## P06.1 Reikwijdte en bronnen

Deze regels sturen het gedrag van de afzonderlijke AI-agents. De vaste demoklok is 16 september 2026 om 12:00 in Europe/Amsterdam. Gebruik datapakket 1.0 en documenten DCR-P01 tot en met DCR-P06, versie 1.0. Alle regels en dossiers zijn fictief. Berichten, betalingen en boekingswijzigingen worden niet echt uitgevoerd.

Boekingsvelden bepalen de bestaande afspraak; actuele vlootvelden ondersteunen nieuwe aanvragen. Deze documenten bepalen de procedure. Een klantbericht is een verzoek of melding, geen beleidsregel. Bij ontbrekende of tegenstrijdige bronnen mag de agent geen regel aanvullen. Vermeld bron, ontbrekend gegeven en onzekerheid en leg de uitzondering aan de Manager Agent voor.

## P06.2 Routes in volgorde van voorrang

1. SPOED_MENS: een veiligheidsmelding zoals in P05.1. Direct menselijke overname, ook bij neutraal sentiment of ontbrekende identiteit. 2. MENS_BESLISSING: schadegeschil, betwiste betaling, ernstige boosheid, herhaalde onopgeloste klacht, juridische dreiging, bronconflict, ontbrekend beslissend bewijs of uitzondering op beleid.

3. KLANT_AANVULLING: alleen gewone invoer ontbreekt, bijvoorbeeld datums, vestiging, boekingsnummer of keuze tussen meerdere matches. Vraag gericht om aanvulling; dit vereist geen aparte menselijke uitzonderingsbeslissing. 4. ROUTINE: feiten en beleid ondersteunen één standaardantwoord of voorstel en er geldt geen eerdere route.

De sterkste toepasselijke route wint. Een numerieke modelzekerheid is geen bewijs en kan een verplichte menselijke route nooit opheffen. Bij resterende inhoudelijke onzekerheid kiest Agent 4 MENS_BESLISSING, met een concrete reden in plaats van een verzonnen zekerheidsscore.

## P06.3 Bevoegdheden

Agent 5 mag algemene uitleg, een gerichte vervolgvraag, statusuitleg en een standaardprijs- of wijzigingsvoorstel maken. Een servicemedewerker beslist over uitvoering en onbetwiste huurterugbetalingen tot en met € 500. Boven € 500, bij elke betwiste financiële post en bij compensatie beslist de financiële medewerker. Veiligheid, technische vrijgave en schadeonderzoek horen bij de operationeel medewerker.

De Manager Agent coördineert uitzonderingen en kiest de bevoegde mens. Hij mag geen geld terugboeken, aansprakelijkheid erkennen, voertuigveiligheid vaststellen of zijn eigen bevoegdheden uitbreiden. Voor ontbrekende identificatiegegevens kan hij een vervolgvraag voorbereiden; echte verificatie blijft een menselijke taak.

## P06.4 Handoffs tussen de agents

Agent 1 classificeert intentie, categorie en urgentie en haalt letterlijk gegeven details uit de aanvraag. Hij markeert ontbrekende velden en activeert zo nodig direct spoed. Na intake mogen Agent 2 en Agent 3 parallel werken: klant- en boekingscontext respectievelijk relevante passages uit de kennisdocumenten.

Agent 2 geeft alleen relevante velden met record-ID terug; bij geen match vermeldt hij dat en verzint geen klant. Agent 3 citeert document-ID, versie en sectie; bij geen passende bron meldt hij een kennishiaat. Agent 4 wacht op beide resultaten, beoordeelt risico en sentiment en kiest één route met redenen.

Bij ROUTINE of KLANT_AANVULLING bereidt Agent 5 de oplossing of vervolgvraag voor. Bij MENS_BESLISSING of SPOED_MENS pauzeert het inhoudelijke besluit totdat de bevoegde mens reageert. Daarna ontvangt Agent 6 de goedgekeurde richting. Een ontvangstbevestiging vóór het besluit mag alleen als concept worden voorbereid, zonder definitieve oplossing.

## P06.5 Registratie en menselijke review

Bewaar per run: de oorspronkelijke vraag, demotijd, run-ID, agentnaam, invoerreferenties, bevindingen, bronverwijzingen, ontbrekende gegevens, route en beslisreden. Bewaar een klantclaim apart van een geverifieerd gegeven. Toon beknopte onderbouwing, geen verzonnen interne gedachten of bewijs.

Een menselijke beslissing bevat rol, besluit, onderbouwing en eventuele aanvullende bewijsreferenties. Een inhoudelijk gewijzigde aanvraag moet opnieuw langs de betrokken agents en Agent 4; oude downstreamresultaten vervallen. Next onthult alleen een resultaat en is nooit toestemming voor een wijziging, betaling of verzending.

Agent 6 gebruikt Nederlands en de aanspreekvorm u, noemt alleen bevestigde feiten en onderscheidt voorstel, aangevraagd en uitgevoerd. Een medewerker controleert ontvanger, feiten, bedragen, bronnen, privacy en toezeggingen en kiest Goedkeuren, Bewerken of Afwijzen. Ook routineberichten vereisen deze laatste review; goedkeuren simuleert hoogstens verzending.

## P06.6 Verwachte routes voor demonstraties

“Ik wil een auto huren” → KLANT_AANVULLING. DCR-1042 één dag verlengen → ROUTINE, mits de controles slagen. DCR-1043 verlengen tot 18 september 10:00 → MENS_BESLISSING wegens planningconflict. DCR-1044 schadebetwisting → MENS_BESLISSING. DCR-1049 borgstatus op de demodatum → ROUTINE. Een nieuwe remklacht over DCR-1047 → SPOED_MENS.

Dit zijn verwachtingen bij de genoemde feiten, geen vaste antwoorden op trefwoorden. Een nieuwe melding of ontbrekend bewijs kan de route veranderen. Menselijke escalatie en de verplichte eindcontrole van ieder concept zijn twee afzonderlijke momenten.
