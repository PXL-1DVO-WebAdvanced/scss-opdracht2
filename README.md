# SCSS: Opdracht 2

Deze opdracht is het vervolg van opdracht 1: https://classroom.github.com/a/2Cllv-2l

## 1. Setup
Net zoals in de vorige opdracht moet je ook nu een lokale clone maken van deze repository!
Omdat we voor deze opdracht een nieuwe repository aanmaken moeten we ook het sass package opnieuw installeren. 
In de startbestanden zit echter al een package.json bestand met een verwijzing (*dependency*) naar het sass package. 
In dit geval volstaat het om het 'npm install' commando uit te voeren in de terminal, hierdoor zullen alle packages worden geïnstalleerd in de node_modules folder.
    
    npm install

## 2. HTML
Maak in het index.html bestand, binnen de body tag, volgende elementen aan:
- Een nav element die je de klasse “nav” geeft. 
  - Binnen dit element voorzie je een ongeordende lijst. Definieer in deze lijst een aantal lijstitems. 
  - Binnen elk item zit telkens een anchor link die linkt naarde huidige pagina.
- Een section element met een klasse “banner”. 
  - Dit element bevat een heading van niveau 1 en een paragraaf. Geef de elementen content naar keuze.
- Een footer element met een klasse “footer”. 
  - Dit element bevat een heading van niveau 3 en eenparagraaf. Geef de elementen content naar keuze

## 3. Variabelen
De HTML pagina stelt de website voor. Deze website zal hoofdzakelijk drie kleuren gebruiken. Om vooreenheid te zorgen in de lettergrootte, gaan we deze ook definiëren.
Verwijder de bestande code in het main.scss bestand maak dan de volgende 6 variabelen aan en geef ze een waarde:
- 3 Variabelen voor de verschillende kleuren
  - primary-color: red
  - secondary-color: blue
  - tertiary-color: yellow
- 3 Variabelen voor de lettergrootte:
  - font-lg: 70px
  - font-md: 50px
  - font-sm: 24px

Pas vervolgens het volgende toe:
- Gebruik de primary-color variabele om het nav-element, op basis van de klasse, een achtergrondkleur te geven.
- Geef het heading element binnen het element met klasse “banner” de volgende eigenschappen:
  - Lettergrootte: font-lg
  - Tekstkleur: secondary-color
  - Gecentreerde tekst
- Geef het heading element in de footer volgende eigenschappen:
  - Lettergrootte: font-md
  - Tekstkleur: primary-color
  - Gecentreerde tekst
 
Bekijk de code nu in het main.css bestand en vergelijk deze met die in het main.scss bestand.

