# Betaling en borg

Document-ID: DCR-P04
Versie: 1.0
Geldig vanaf: 2026-09-01
Herziening: 2026-12-01
Eigenaar: Financiële administratie
Taal: nl-NL
Tags: betaling, borg, terugbetaling, factuur

Fictieve bedrijfsregels voor de demonstratie. Geen echte verhuurovereenkomst.

## P04.1 Huurbetaling en uitgifte

Deze instructie houdt huurbetalingen, terugbetalingen en borg uit elkaar. De huur moet vóór uitgifte betaald zijn. Een bevestigde reservering mag nog een openstaande huurbetaling hebben. Agent 2 rapporteert de geregistreerde status; de AI vraagt nooit kaartgegevens of een beveiligingscode via het bericht.

In de demo kan de medewerker betaling via iDEAL of betaalkaart registreren. Voor de borg wordt een reservering op een geschikte betaalkaart van de hoofdbestuurder gebruikt. Een alternatieve betaalwijze vraagt een medewerker. De AI maakt geen betaallink of bankrekeningnummer aan.

## P04.2 Bedragen interpreteren

huursom_eur is de afgesproken huurprijs. betaald_eur is de cumulatief geregistreerde huurbetaling; terugbetaald_eur is de cumulatieve huurterugbetaling. Deze bedragen bevatten geen borg. De oorspronkelijke huursom blijft ook bij een geannuleerde boeking zichtbaar voor de historie.

borg_eur is de afgesproken zekerheid. borg_vastgehouden_eur geeft de nog gereserveerde of ingehouden zekerheid weer. Een borgreservering is niet hetzelfde als een afschrijving of huurbetaling. betwiste_schade_eur is een betwist bedrag en bewijst geen vastgestelde schuld.

## P04.3 Borgstatus lezen

Nog niet gereserveerd betekent dat de borgcontrole vóór uitgifte nog moet plaatsvinden. Gereserveerd betekent dat zekerheid is vastgelegd. Vrijgave aangevraagd betekent dat een opdracht is gegeven maar bankverwerking nog niet is bevestigd. Vrijgegeven betekent dat de administratie de vrijgave bevestigt.

Deels ingehouden betekent dat een deel nog vaststaat. Niet van toepassing geldt bijvoorbeeld bij een niet-bevestigde optie of een vóór uitgifte geannuleerde huur zonder borg. Leid een daadwerkelijke bankafschrijving nooit alleen uit deze labels af.

## P04.4 Vrijgave en termijnen

Bij een retour zonder openstaande afwijkingen vraagt de medewerker uiterlijk binnen twee werkdagen vrijgave van de borg aan. Voor deze demo zijn werkdagen maandag tot en met vrijdag; Nederlandse feestdagen zijn niet gemodelleerd. Een termijn begint op de eerstvolgende werkdag na de relevante gebeurtenis.

Na de vrijgaveopdracht is de verwachte verwerking drie tot vijf werkdagen, afhankelijk van de bank. Dit is een fictieve servicetermijn en geen garantie. Bij uitblijven na vijf werkdagen, een ontbrekende opdracht na twee werkdagen of tegenstrijdige status gaat de zaak naar de financiële medewerker via de Manager Agent.

## P04.5 Terugbetalingen en geschillen

Een huurterugbetaling vereist een verklaarde grondslag, het te restitueren bedrag, controle op eerdere terugbetaling en menselijke goedkeuring. Tot en met € 500 kan de bevoegde servicemedewerker goedkeuren; boven € 500 is de financiële medewerker nodig. Elke betwiste betaling of borginhouding gaat naar de financiële medewerker, ongeacht het bedrag.

De AI kan een berekening en conceptantwoord voorbereiden, maar doet geen financiële boeking. Zonder uitvoeringsbevestiging schrijft Agent 6 “voorgesteld” of “aangevraagd”, niet “terugbetaald”. Bij een betwiste schadepost geldt ook DCR-P05. Maak geen verrekening op basis van alleen een klantclaim of interne notitie.

## P04.6 Voorbeelden uit de dataset

DCR-1046 heeft € 267 huur, € 0 betaald en nog geen borgreservering. De reservering is bevestigd, maar de auto kan pas na de uitgiftecontroles worden meegegeven.

Voor DCR-1049 is € 1.000 borg nog zichtbaar als vastgehouden. De vrijgave is 15 september aangevraagd; op de demodatum 16 september is geen overschrijding aangetoond. De AI mag niet zeggen dat de bank de borg al heeft vrijgegeven.

Bij DCR-1044 is van € 500 borg nog € 350 vastgehouden wegens betwiste schade; € 150 is vrijgegeven. Er is € 165 huur betaald. Deze drie bedragen mogen niet worden samengevoegd tot één openstaande huurschuld.
