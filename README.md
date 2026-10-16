# de3biggetjes.nl

Statische site voor De 3 biggetjes, de musical van B&M Entertainment (gespeeld op 10 en 11 oktober 2026 in Stadstheater Zoetermeer). Gebaseerd op de build van het online programmaboekje.

## Deployen op Vercel

Importeer deze repo in Vercel met framework preset **Other**. Er is geen build-stap en de output directory is de root.
Koppel `de3biggetjes.nl` als hoofddomein en `www.de3biggetjes.nl` als extra domein. `vercel.json` stuurt www door naar het kale domein.

## Structuur

- `index.html`: de hele site (secties: verhaal, cast, muziek, quiz, herberg, foto's, team, producties, terugblik, FAQ en contact)
- `privacyverklaring.html` en `404.html`: losse pagina's in dezelfde stijl
- `css/site.css`: alle styling, inclusief de vuurvliegjes-achtergrond (`.vliegjes`)
- `_astro/*.js`: interactie (cast-pop-ups, muziekfilter, quiz, navigatie, delen)
- `img/`, `fonts/`: afbeeldingen en lettertypen

Het contactformulier is een Tally-embed (formulier `nPGaxB`).

## Aanpassen

Teksten staan direct in de HTML. Vervang je een afbeelding onder `img/` met dezelfde bestandsnaam, dan zien bezoekers de nieuwe versie binnen een dag (cache-instelling in `vercel.json`).
