# Verkeersborden-App
[![Het gerealiseerde eindproduct op desktop](https://vettedingenbouwen.nl/img/verkeersborden.png)](https://vettedingenbouwen.nl/video/verkeersborden/promo.mp4) 
<i>Klik op de video hierboven voor een demo!</i>

Een deel van deze app is gemaakt voor de IT-Proeverij van 21-September-2021 voor Code Café. Deze app biedt een informatieve manier om verkeersborden te leren. Ook heb ik aan deze app gewerkt in mijn eigen tijd. De versie die tijdens de demo is gemaakt is eigendom van code-café. 

## Intro
Leer de betekenis van verkeersborden met deze handige app! Over over de verschillende kaartjes voor het antwoord.

## Uitleg IT-proeverij
Tijdens deze proeverij leer je de basis van "css-art" om verkeersborden te maken aan de hand van de Block-Element-Modifier (BEM) methodiek. Deze methodiek zorgt ervoor dat je geen CSS-breekt wanneer je iets wilt hergebruiken en/of modificeren. 
Alle info is afkomstig van https://www.informatiebord.nl/oefenen/verkeersborden-overzicht/. 

### Promo Video
https://www.youtube.com/watch?v=qmFKxBbZzzU

### IT-Proeverij 21-September-2021
https://www.youtube.com/watch?v=qmFKxBbZzzU

<b>De app is absoluut niet bedoeld voor commericeel gebruik.</b>

## Dingen die ik heb geleerd 
1. Box-shadow is enorm handig voor het maken van meerdere borders. Zoals verkeersborden met een rode -> witte -> rode rand. 
2. Dikte van borders kan je opgeven door de spread van de vorige box-shadow te gebruiken. Bijv: 2.5rem (25 px) is de vorige spread van de border (dikte van de rand), als je hierna een 0.5 (5px) border wilt zal je deze 25 + 5 => 30px moeten maken (de spread).
3. Ik heb geleerd hoe backface visibility werkt en wat het precies is.
4. Met de kennis uit 3) heb ik een kaartje kunnen maken die zichzelf omdraait en dan content laat zien.
5. Ik heb het kaartje gerealiseerd door de achterkant op de voorkant te leggen en in het begin om te draaien. Door backface visibility op hidden te zetten wordt deze pas getoond als het kaartje omdraait. 
6. Punt 5 had "logischer" gerealiseerd kunnen worden door de voorkant op de achterkant te laten liggen en het kaartje in zijn geheel om te laten draaien.
7. Opnieuw gezien hoe ongeloofelijk makkelijk het is om met flexbox een responsive layout te maken.
8. Geleerd dat wanneer je een groot scherm hebt (mijn scherm is zo'n 3400px breed) is het belangrijk max-width op een wrapper toe te voegen. Kan eventueel ook met auto-fit / auto-fill op een CSS-Grid in combinatie met repeat. Zie de code hieronder, hiermee maak je zoveel mogelijk columns van 200px.  
    <code>
        grid-template-columns: repeat(auto-fit,200px);
    </code>
9. Geleerd wat het verschil is tussen auto-fit en auto-fill op basis van onderzoek naar punt 8. auto-fill vult lege rijen met lege columns aan als dit past. auto-fit zorgt ervoor dat de grid columns groter maakt. Let op dat wanneer je repeat met minmax gebruikt zowel bij auto-fill als auto-fit de columns groeien. Maar dat auto-fill op een gegevens moment bij genoeg breedte lege columsn toevoegd. 
10. Hoe tabindex gebruikt kan worden en waarom groter dan 0 niet wenselijk is (omdat je de natuurlijke order van html breekt). 
11. Geleerd dat backface-visiblity: hidden bugs geeft op safari (zucht). Kan gefixed worden door  translateZ(1px) toe te voegen aan transforms.
12. Geleerd hoe je een kaartje in 3D kan laten draaien. Dit doe je door een <code> transform: perspective(100rem); </code> toe te voegen. Ik gebruikte dit in eerste instantie om de flickerin na een <code> transform: scale(); </code> weg te halen, maar dit gaf een verrassend leuk effect! Met de perspective property kreeg ik het niet voor elkaar, maar wel met de transform. Zoals ik het nu snap geeft perspective de kinderen in het element een perspectief, transform zorgt dat het element zelf een perspectief krijgt. 
13. Geleerd dat preserve-3d gebruikt dient te worden op een element om deze goed te laten renderen in 3d. De properties werkt op de geneste elementen. 

## Screenshots
Hieronder zijn een aantal screenshots toegevoegd van de app op verschillende devices.

### Desktop Screenshot
![Het gerealiseerde eindproduct op desktop, 4 kaartjes naast elkaar](https://vettedingenbouwen.nl/img/verkeersborden.png "Verkeersborden-App")

### Mobile Screenshot
![Het gerealiseerde eindproduct op mobiel, 2 kaartjes naast elkaar](https://vettedingenbouwen.nl/img/verkeersborden_mobile.png "Verkeersborden-App")

## Live demo
https://vettedingenbouwen.nl/verkeersborden

## Resources
1. Resource gebruikt voor het leren van het verschil tussen auto-fit en auto-fill. https://css-tricks.com/auto-sizing-columns-css-grid-auto-fill-vs-auto-fit/
2. Resource gebruikt voor het leren van perspective. https://www.w3schools.com/CSSref/css3_pr_perspective.asp
3. Post gebruikt om het verschil tussen perspective and transform: perspective te snappen. https://stackoverflow.com/questions/25910933/what-is-the-difference-between-perspective-and-transforms-perspective-propertie
4. Resource gebruikt om preserve-3D te snappen. https://www.w3schools.com/CSSref/css3_pr_transform-style.asp
