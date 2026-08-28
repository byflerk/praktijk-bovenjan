# praktijk-bovenjan.nl

De website van Praktijk Boven Jan — Jan Roelofsen, relatie- en persoonlijk coach.

## Wat dit is

Losse HTML. Geen framework, geen build, geen dependencies.
Twee bestanden zijn de hele site:

- `index.html` — de pagina zelf (styling en scripts zitten erin)
- `foto-jan.jpg` — de foto in de hero

Je opent `index.html` gewoon in een browser om te kijken. Er is niets te
installeren en niets te compileren.

## Publiceren

Cloudflare is gekoppeld aan deze repository. Elke push naar `main` zet de
site automatisch live op praktijk-bovenjan.nl. Er is geen buildstap:
Cloudflare serveert de map zoals hij is.

## Twee dingen die ingevuld moeten worden

1. **Web3Forms-sleutel** — zoek in `index.html` op `PLAK-HIER-JE-ACCESS-KEY`.
   Zolang die er staat opent het contactformulier de mailclient van de
   bezoeker in plaats van te versturen.

2. **Bedrijfsgegevens in de footer** — KvK-nummer, BTW-id en adres.
   Wettelijk verplicht op een zakelijke site.

## Onderhoud

- De startdatum van de Houd me Vast-groep staat hard in de pagina.
  Zoek op `29 sept 2026` en werk die per groep bij.
- Het Houd me Vast-blok is bewust los te knippen: alles tussen de twee
  comments `HOUD ME VAST` en `EINDE HOUD ME VAST` kan eruit zonder dat er
  elders iets stukgaat.

## Getest

320 tot 1440 px, geen horizontale overloop. Werkt zonder JavaScript
(animaties uit, inhoud zichtbaar) en respecteert "beperk beweging".
