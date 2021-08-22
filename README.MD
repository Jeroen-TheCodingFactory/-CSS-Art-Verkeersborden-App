Deze app is gemaakt voor de IT-Proeverij van 21-September-2021 voor Code Café. Deze app is een informatieve manier om verkeersborden te leren. 
Tijdens deze proeverij leer je de basis van "css-art" om verkeersborden te maken aan de hand van de Block-Element-Modifier (BEM) methodiek. Deze methodiek zorgt ervoor dat je geen CSS-breekt wanneer je iets wilt hergebruiken en/of modificeren. 
Alle info is afkomstig van https://www.informatiebord.nl/oefenen/verkeersborden-overzicht/.
De app is absoluut niet bedoeld voor commericeel gebruik. 

Dingen die ik heb geleerd:

1) Box-shadow is enorm handig voor het maken van meerdere borders. Zoals verkeersborden met een rode -> witte -> rode rand. 
2) Dikte van borders kan je opgeven door de spread van de vorige box-shadow te gebruiken. Bijv: 2.5rem (25 px) is de vorige spread van de border (dikte van de rand), als je hierna een 0.5 (5px) border wilt zal je deze 30 - 5 => 25 rem moeten maken (de spread).
3) Ik heb geleerd hoe backface visibility werkt en wat het precies is
4) Met de kennis uit 3) heb ik een kaartje kunnen maken die zichzelf omdraait en dan content laat zien.
5) Ik heb het kaartje gerealiseerd door de achterkant op de voorkant te leggen en in het begin om te draaien. Door backface visibility op hidden te zetten wordt deze pas getoond als het kaartje omdraait. 
6) 5) had "logischer" gerealiseerd kunnen worden door de voorkant op de achterkant te laten liggen en het kaartje in zijn geheel om te laten draaien.
7) Opnieuw gezien hoe ongeloofelijk makkelijk het is om met flexbox een responsive layout te maken.
8) Geleerd dat wanneer je een groot scherm hebt (mijne is zo'n 3400px breed) is het belangrijk max-width op een wrapper toe te voegen. 
9) Hoe tabindex gebruikt kan worden en waarom groter dan 0 niet wenselijk is (omdat je de natuurlijke order van html breekt). 
