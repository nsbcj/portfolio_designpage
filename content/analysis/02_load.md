---
Title: Load
icon: fas fa-spinner
---

Rapport - Analys laddningstider
=======================

Bakgrunden till rapporten är en [uppgift](https://dbwebb.se/uppgift/utvardera-webbplatsers-laddningstider-och-anvandbarhet-v2) inom en kurs i webbdesign på BTH.

Uppgiften består av att tre webbplatser ska analyseras utifrån deras laddningstid. Analysen har gjorts baserat på verktyget [PageSpeed Insights](https://pagespeed.web.dev/).

Rapporten är skriven enskilt.

Urval
-----------------------

Urvalet avser samma webbplatser som analyserades i föregående kursmoment. Det kan vara intressant att se hur webbplatserna, relaterade till ämnet design, förhåller sig till prestanda. Gemensamt för webbplatserna är att de innehåller verktyg som underlättar designprocessen.

Följande är en sammanställning av urvalet:

|   Webbplats          |    Mätdatum       |
|   ---------          |     -----      |
|   www.figma.com      |    2022-11-17  |   
|   www.adobe.com      |    2022-11-17  |
|   www.sketch.com     |    2022-11-17  |

Metod
-----------------------
Precis som i föregående analys, kan metoden liknas vid en förenklad fallstudie. Undersökningen har genomförts i följande steg:

1. Webbplatserna har mätts i verktyget PageSpeed Insights. Både mobil- och desktop versionerna har mätts. De betyg verktygen erhållits har noterats i ett kalkylblad.
2. Laddningstid och antal resurser har mätts i dev-tools. Mätvärdet utgörs av ett snittvärde av tre mätningar. Mätvärdena har presenterats i kalkylblad tillsammans med de genomsnittliga värdena. De värde som skrivits in baseras på antalet requester, mängden nedladdad data samt värdet "load" i nätverksfliken. Anledningen till att "load" valts som riktvärde, var att vissa webbplatser upplevdes fortsätta ladda innehåll även efter att hela sidans innehåll visats på webbplatsen.
3. En sammansfattning har skrivits om vilka förbättringsmöjligheter som finns på respektive sida.
4. Resultaten har sammanfattats i en analys där de vanligaste förbättringsåtgärderna noterats, tillsammans med iakttagelser av intresse i resultatet.
5. Webbplatserna har slutligen rangordnats utifrån en samlad bedömning.
6. Slutligen har min uppfattning om vad som är en tillräckligt laddningstid noterats.

Material
-----------------------
LePage (2014, uppdaterad 2020) beskriver att bilder ofta det kräver mest utrymme vid nedladdning av en webbplats. 60% av det som laddas vid visande av en webbplats upptas av bilder. Vidare beskriver han fyra tips för att kombinera optimering och användarupplevelse vid inladdning av bilder. De fyra delar han nämner är; användande av relativ bildstorlek, picture-element, srcset och x i img-element (för att välja rätt pixel-densitet för användare) samt användande av inline-images för att minska antalet anrop på filer. Ett exempel på det sistnämnda är svg-filer som kan skrivas inline.

Webbplatsen MOZ (https://moz.com/learn/seo/page-speed) beskriver vad page speed är och hur man kan reducera laddningstider. Följande är delar som omnämns minska laddningstider:
* Möjliggöra att filer kan komprimeras.
* Minifiering av Html-, Css- och JavaScript-filer optimerar sidan genom att ta bort onödig information i filerna.
* Ett minskat antal requests internt på webbplatsen.
* Borttagande av onödiga script-block med Javascript i Html-elementet.
* Optimera serverns responstid.
* Användande av CDNs (content delivery networks), för att användare ska få snabbare och bättre tillgång till webbplatsen.
* Optimera bilder, genom att använda rätt typ av filer. Jpg, eller jpeg, är bäst för fotografier medan png beskrivs vara bra för grafik.

Verktyget PageSpeed beskrivs mäta en rad parametrar kopplade till en webbplats prestanda. Den parameter som bedömts central i resultatet är webbplatsens prestanda (performance).

Resultat
-----------------------
*Förklaringar kopplat till förkortningar i kalkylbladet:*

*FCP - First Contentful Paint, TTI - Time to Interactive, SI - Speed Index, TBT - Total Blocking Time, LCP - Largest Contentful Paint, CLS - Cumulative Layout Shift.*

*Resurser är mätta i antal, tid i sekunder och storlek i mb.*

###Kalkylblad

<div class="embed-container">
    <iframe src="https://ethercalc.net/hy4ofxxx9ulw/form" frameborder="0"></iframe>
</div>

###Förbättringsmöjligheter

Enligt PageSpeed kan Figma reducera andelen oanvänd Javascript och reducera serverns responstid för att förbättra sidan.

Enligt PageSpeed kan även Adobe reducera andelen oanvänd Javascript samt oanvänd CSS, men även minska andelen innehåll som blockerar sidans rendering.

Förutom att reducera mängden oanvänd Javascript kan Sketch förbättra hanteringen av bilder på sidan. Bland annat genom att använda lazy-loading, så att inte bilder laddas in när de inte är i användarens vy. Sidan ska även ta bort resurser som blockerar renderingen.

Analys
-----------------------
Det har varit intressant att använda verktyget PageSpeed. Det är också intressant att jämföra resultaten från PageSpeed med de mätvärden som hämtades från dev-tools. Moz-artikeln tar upp flera av de förbättringsmöjligheter som PageSpeed-mätningarna genererat. Att reducera mängden oanvänd Javascript i kombination med att minska andelen innehåll som blockerar sidans rendering, verkar vara de främsta förbättringsmöjligheterna avseende de tre sidor som ingår i mätningarna. Bildhanteringen förefaller, med undantag från Sketch, vara bra.

Det som stack ut i prestandamätningarna var att Adobe fick förhållandevis låga poäng i mobil-versionen. Tittar man på resultatet så ser man att sidans uppmätta tider är långa avseende allt utom FCP (first contentful paint) och LCP (largest contentful paint). Siffrorna för Adobe är något bättre i desktop-versionen. Jämför man med Adobes resultat för laddade resurser ser man å andra sidan att webbplatsen har bäst resultat avseende både antalet laddade resurser, laddningstid och storlek. Detta skulle möjligen kunna förklaras av hur mätningen är gjord och valet av värden som gjorts från dev-tools. Det är dock även en möjlighet att Adobes prestanda påverkas av att de har innehåll som blockerar sidans rendering. I sådant fall skulle borttagande av innehåll som blockerar sidans rendering möjligen ha positiv effekt på sidans prestandapoäng.

Figma, som har relativt höga poäng avseende både mobil- och desktop-prestanda, laddar å andra sidan många resurser och en stor mängd data. En avvikelse som noterats är att Figma vid den andra mätningen, endast laddade 6.3 mb i förhållande till det genomsnittliga 15.51 mb. Vid denna mätning laddades också ett färre antal resurser från webbplatsen.

Sketch har en laddningstid som var mer en dubbelt så lång i förhållande till de andra två webbplatserna. Å andra sidan har Sketch den högsta poängen avseende prestanda. Sketch prestanda i desktop versionen uppgåt till 86, vilket är uppfattas vara bra.

En tydlig tendens i resultatet av undersökningen är att samtliga webbplatser fungerar bättre på desktop än i mobilen. Kanske det kan säga något om företagens målgrupp. Webbplatserna är ur detta hänseende optimerade för desktopanvändare. Det skulle vara intressant att se statistik över hur många besök som på desktop- respektive mobil versionerna, för att sedan se hur det speglar prestandamåtten.

###Rangordning baserat på mätvärde
Den webbplats som har övergripande bäst resultat är Figma. Figma har den bästa mobila prestandan, den näst bästa prestandan för desktop och den lägsta laddningstiden. Dock laddar sidan mest data, vilket möjligtvis drar ner det övergripande betyget något.

 De låga poängen Adobe erhöll på PageSpeed bedöms motivera att Sketch har en generellt bättre prestanda. Det bör dock nämnas att Adobe laddar minst antal resurser, minst data och har en snabb laddningstid. Adobe är enligt undersökningen bättre än Sketch på dessa tre punkter. Sketch har dock bättre poäng avseende både mobil- och desktop prestanda, varvid det anses utgöra grund för att Sketch kommer strax före Adobe.

| Bild |   Webbplats          |    Plats       |
|----- |   ---------          |     -----      |
|  ![Bild kunde inte laddas](../image/figma.png?h=100&save-as=jpg&q=40) |   www.figma.com      |    1  |   
|  ![Bild kunde inte laddas](../image/sketch.png?h=100&save-as=jpg&q=40) |   www.sketch.com     |    2  |  
|  ![Bild kunde inte laddas](../image/adobe.png?h=100&save-as=jpg&q=40) |   www.adobe.com      |    3  |

###Avseende laddningstider
Känslan är att man bör understiga fyra-fem sekunders laddningstid. Som det beskrivs i en av artiklarna, *“Google Developers: Why Performance Matters”* (Pavix, Anstey, Wagner 2019 uppdaterad 2020), påverkar laddningstiden intresset för sidan. Att fort se relevant innehåll kanske till och med överväger intresset att mötas av en god design. En annan sak som påverkar helhetsintrycket är pop-up rutor som dyker upp efter laddningen. I vissa fall kan det uppfatts som negativt att det efter fem sekunder kommer upp en ruta, likt på Adobes webbplats.

Trots att Sketch överskrider gränsen ovan är känslan att sidan laddar ganska snabbt. Kanske beror det på att det viktigaste innehållet laddas snabbt. Både Figma och Adobe, ger en känsla av att laddningen går tillräckligt fort.

Referenser
-----------------------
LePage, Pete. 2014 (uppdaterad 2020). *"Responsive images"*; https://web.dev/responsive-images/. Läst 2022-11-18.

Pavic, Bojan; Anstey, Chris; Wagner, Jeremy; 2019 (uppdaterad 2020). *“Google Developers: Why Performance Matters”*. https://web.dev/why-speed-matters/. Läst 2022-11-21.

*"Page-speed"*. https://moz.com/learn/seo/page-speed. Läst 2022-11-18.

*"PageSpeed Insights"*. https://pagespeed.web.dev/. Mätning gjord 2022-11-17.

Övrigt
-----------------------
Författare: anjc20
