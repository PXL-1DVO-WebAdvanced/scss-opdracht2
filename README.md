# SCSS: Opdracht 2

Deze opdracht is het vervolg van opdracht 1: https://classroom.github.com/a/2Cllv-2l

## 1. Setup
Net zoals in de vorige opdracht moet je ook nu een lokale clone maken van deze repository!
Omdat we voor deze opdracht een nieuwe repository aanmaken moeten we ook het sass package opnieuw installeren. 
In de startbestanden zit echter al een package.json bestand met een verwijzing (*dependency*) naar het sass package. 
In dit geval volstaat het om het 'npm install' commando uit te voeren in de terminal, hierdoor zullen alle packages worden geïnstalleerd in de node_modules folder.
    
    npm install

Wanneer het sass package geïnstalleerd is kunnen we ook het dev script opnieuw uitvoeren:

    npm run dev

## 2. HTML
Verwijder de inhoud van het index.html bestand en maak, binnen de body tag, volgende elementen aan:
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

## 4. Nesting
Gebruik nesting om:
- Het bullet point van het list-item binnen het nav element weg te halen
- De basisstijl van de anchor-link binnen dat list-item wordt weggehaald. Gebruik verder de eerder gedefinieerde variabelen om de lettergrootte en de tekstkleur aan te passen. (font-md + tertiary-color)
- Zorg er met een hover effect voor dat de tekstkleur van de anchor-link binnen het list-item wijzigt naar de secondary-color

## 5. Mixin
Maak een mixin 'margin-padding' die ervoor zorgt dat de elementen nav, section en footer een margin en padding krijgen van 3px. 
Gebruik waar het kan de klasse namen.

### Parameter
Pas de mixin aan zodat je er een argument aan kan meegeven. Dit argument is de waarde voor de padding.
Voor de nav is dat 5px, voor de section 3px en de footer 3px;

### Parameter...
Definieer een hover effect binnen het footer element (gebruik hiervoor nesting). 
Zorg ervoor dat detekstkleur en de achtergrondkleur wijzigt.
Vervolgens pas je een transition toe op de kleur van 0,5s én op de achtergrondkleur van 1s. 
Maak hiervoor gebruik van een mixin waarbij je meerdere waardes kan meegeven als argument.

## 6. Extend
Maak een klasse “background-primary” (die in de HTML niet zal gebruikt worden) met volgende eigenschappen:
- Achtergrondkleur naar keuze.
- Tekstkleur naar keuze.
- Gecentreerde tekst.

Pas deze stijl via een extend toe op alle paragrafen.

## 7. Functies
Maak een functie “increaseFontSize”. 
Deze functie heeft een parameter $size en geeft de waarde hiervan, vermenigvuldigd met 2, terug.
Roep deze functie aan in de paragrafen voor de lettergrootte

## 8. Partials
Voeg volgende partials toe:
- _global: met alle variabelen, mixins, functies en overkoepelende stijlen.
- _nav: met alle code voor de navigatie.
- _section: met alle code voor het section element.
- _footer: met alle code voor het footer element.

Zorg ervoor dat al deze partials ingeladen worden in het main.scss bestand. 

