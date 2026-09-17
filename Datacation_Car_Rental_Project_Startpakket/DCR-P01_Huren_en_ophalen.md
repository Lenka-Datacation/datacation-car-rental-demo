# Huren en ophalen

Document-ID: DCR-P01
Versie: 1.0
Geldig vanaf: 2026-09-01
Herziening: 2026-12-01
Eigenaar: Verhuuroperatie
Taal: nl-NL
Tags: nieuwe huur, ophalen, rijbewijs, identificatie

Fictieve bedrijfsregels voor de demonstratie. Geen echte verhuurovereenkomst.

## P01.1 Doel en benodigde gegevens

Deze werkinstructie beschrijft hoe Datacation Car Rental een huuraanvraag voorbereidt en een auto uitgeeft. Een algemene vraag mag zonder klantrecord worden beantwoord. Een reservering wordt pas definitief nadat de vereiste controles zijn afgerond.

Vraag bij een nieuwe aanvraag naar de ophaalvestiging, ophaal- en inleverdatum met tijd, gewenste autoklasse of model en eventuele extra bestuurder. Vraag voor de reservering ook naam en e-mailadres. Verzin geen datums, locatie of voertuigvoorkeur. Vraag bij “volgende vrijdag” welke datum wordt bedoeld als dit niet eenduidig is.

## P01.2 Voorwaarden voor bestuurders

Voor deze demo geldt voor alle tien auto’s: minimaal 21 jaar bij ophalen, minimaal één jaar in bezit van rijbewijs B en een geldig rijbewijs en identiteitsdocument bij uitgifte. Er geldt geen jongebestuurderstoeslag. Dit zijn fictieve bedrijfsvoorwaarden, geen beschrijving van Nederlandse wettelijke eisen.

Bereken leeftijd en rijbewijsduur op de ophaaldatum. De datum rijbewijs_sinds bewijst niet dat het rijbewijs nog geldig is. De medewerker controleert geldigheid en geschiktheid aan de balie. Een extra bestuurder moet dezelfde controles doorlopen. Vraag in het bericht geen BSN, documentkopie, kaartnummer of beveiligingscode.

## P01.3 Klant en boeking terugvinden

Agent 2 zoekt op boeking_id of een exact e-mailadres en koppelt via klant_id en auto_id. Alleen een naam is geen betrouwbare unieke identificatie. Bij meerdere boekingen vraagt het systeem welke boeking wordt bedoeld.

Een gevonden record of de waarde Geverifieerd is geen bewijs dat de huidige afzender die klant is. Voor de fictieve demonstratie bevestigt de presentator de gekozen klantrol. Zonder die bevestiging geeft het systeem alleen algemene informatie of vraagt het om verduidelijking; het deelt geen persoonsgebonden financiële details.

## P01.4 Vestigingen en beschikbaarheid

De fictieve verhuurpunten in Amsterdam, Utrecht en Rotterdam zijn dagelijks open van 09:00 tot 18:00, ook in het weekend. Ophalen en inleveren gebeurt in deze demo bij dezelfde vestiging en binnen die tijden. Een andere vestiging, buitenlandrit of afwijkend tijdstip vraagt beoordeling door de Manager Agent; beloof geen uitzondering.

Controleer de volledige gewenste huurperiode tegen alle lopende huren, bevestigde boekingen, niet-verlopen opties en onderhoud. Plan twee uur voorbereiding na iedere inlevering. Een auto met status Beschikbaar is niet automatisch vrij op een toekomstige datum. Een geplande onderhoudseinddatum is geen gereedmelding.

## P01.5 Boeking en uitgifte

Een prijsvoorstel maakt geen boeking. Een optie houdt de auto tijdelijk vast tot de expliciet vastgelegde vervaltijd; zonder vervaltijd mag de AI geen eigen termijn verzinnen. Bevestigd betekent gereserveerd, niet noodzakelijk betaald. Voor uitgifte moeten huurbetaling, borgreservering, bestuurderscontrole en voertuiggereedmelding afgerond zijn.

Bij uitgifte registreert de medewerker tijd, kilometerstand, brandstofniveau of laadpercentage en bestaande schade, met een uitgifterapport. De klant krijgt uitleg over de auto en de retourafspraak. De demo bevat geen echte ondertekende rapporten; de AI mag die niet als aanwezig voorstellen.

## P01.6 Toepassing op de dataset

DCR-1048 van Emma van den Berg is een optie tot 17 september 2026 om 17:00. Zij voldoet op de geplande ophaaldatum aan de demo-eisen voor leeftijd en rijbewijsduur, maar de identiteitscontrole en bevestiging ontbreken. De optie is dus geen definitieve reservering.

Bij “Ik wil een auto huren” ontbreken in elk geval locatie, periode en voertuigvoorkeur. De juiste vervolgstap is die gegevens uitvragen. Dit is op zichzelf geen menselijke escalatie. Geef als bron DCR-P01 versie 1.0, sectie P01.1.
