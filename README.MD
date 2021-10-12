# Verkeersborden-App
[![Het gerealiseerde eindproduct op desktop](https://vettedingenbouwen.nl/img/verkeersborden.png)](https://vettedingenbouwen.nl/video/verkeersborden/promo.mp4) 
<i>Klik op de video hierboven voor een demo!</i>

Een deel van deze app is gemaakt voor de IT-Proeverij van 21-September-2021 voor Code Café. Deze app is een informatieve manier om verkeersborden te leren. Ook heb ik aan deze app gewerkt in mijn eigen tijd. 

Tijdens deze proeverij leer je de basis van "css-art" om verkeersborden te maken aan de hand van de Block-Element-Modifier (BEM) methodiek. Deze methodiek zorgt ervoor dat je geen CSS-breekt wanneer je iets wilt hergebruiken en/of modificeren. 
Alle info is afkomstig van https://www.informatiebord.nl/oefenen/verkeersborden-overzicht/.

<b>De app is absoluut niet bedoeld voor commericeel gebruik.</b>

## Intro
Leer de betekenis van verkeersborden met deze handige app! Over over de verschillende kaartjes voor het antwoord.

## Dingen die ik heb geleerd 
1. Box-shadow is enorm handig voor het maken van meerdere borders. Zoals verkeersborden met een rode -> witte -> rode rand. 
2. Dikte van borders kan je opgeven door de spread van de vorige box-shadow te gebruiken. Bijv: 2.5rem (25 px) is de vorige spread van de border (dikte van de rand), als je hierna een 0.5 (5px) border wilt zal je deze 30 - 5 => 25 rem moeten maken (de spread).
3. Ik heb geleerd hoe backface visibility werkt en wat het precies is
4. Met de kennis uit 3) heb ik een kaartje kunnen maken die zichzelf omdraait en dan content laat zien.
5. Ik heb het kaartje gerealiseerd door de achterkant op de voorkant te leggen en in het begin om te draaien. Door backface visibility op hidden te zetten wordt deze pas getoond als het kaartje omdraait. 
6. Punt 5 had "logischer" gerealiseerd kunnen worden door de voorkant op de achterkant te laten liggen en het kaartje in zijn geheel om te laten draaien.
7. Opnieuw gezien hoe ongeloofelijk makkelijk het is om met flexbox een responsive layout te maken.
8. Geleerd dat wanneer je een groot scherm hebt (mijne is zo'n 3400px breed) is het belangrijk max-width op een wrapper toe te voegen. 
9. Hoe tabindex gebruikt kan worden en waarom groter dan 0 niet wenselijk is (omdat je de natuurlijke order van html breekt). 
10. Geleerd dat backface-visiblity: hidden bugs geeft op safari (zucht). Kan gefixed worden door  translateZ(1px) toe te voegen aan transforms.

## Screenshots
Hieronder zijn een aantal screenshots toegevoegd van de app op verschillende devices.

### Desktop Screenshot
![Het gerealiseerde eindproduct op desktop, 4 kaartjes naast elkaar](https://vettedingenbouwen.nl/img/verkeersborden.png "Verkeersborden-App")

### Mobile Screenshot
![Het gerealiseerde eindproduct op mobiel, 2 kaartjes naast elkaar](https://vettedingenbouwen.nl/img/verkeersborden_mobile.png "Verkeersborden-App")

## Live demo
https://vettedingenbouwen.nl/verkeersborden