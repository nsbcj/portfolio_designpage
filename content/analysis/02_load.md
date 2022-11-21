---
Title: Load
icon: fas fa-spinner
---

Rapport - Analys laddningstider
=======================

Bakgrunden till rapporten är en [uppgift](https://dbwebb.se/uppgift/utvardera-webbplatsers-laddningstider-och-anvandbarhet-v2) inom design på BTH.

Uppgiften består av att tre webbplatser ska analyseras utifrån deras laddningstid. Analysen görs baserat på verktyget [PageSpeed Insights](https://pagespeed.web.dev/).

Rapporten är skriven enskilt.

Urval
-----------------------

Urvalet avser de tre webbplatser som analyserades i föregående kursmoments analys. Det kan vara intressant att se hur webbplatserna, relaterade till ämnet design, förhåller sig till prestanda. Gemensamt för webbplatserna är att de innehåller verktyg som underlättar designprocesser.

Följande är en sammanställning av urvalet:

|   Webbplats          |    Datum       |
|   ---------          |     -----      |
|   www.figma.com      |    2022-11-17  |   
|   www.adobe.com      |    2022-11-17  |
|   www.sketch.com     |    2022-11-17  |

Metod
-----------------------
Precis som i föregående analys, kan metoden liknas vid en förenklad fallstudie. Webbplatserna analyseras i följande steg.

1. Webbplatserna mäts i verktyget PageSpeed Insights för både mobile- och desktop-versionerna. De betyg som verktygen genererar noteras i ett kalkylark.

2. Laddningstid och antal resurser mäts i dev-tools. Mätvärdet utgörs av ett snittvärde av tre mätningar. Mätvärdet noteras i kalkylarket. De värde som skrivits in baseras på antalet requester, mängden nedladdad data samt värdet "load" i nätverksfliken. Anledningen till att "load" valts som riktvärde, är att vissa webbplatser upplevdes fortsätta ladda innehåll även efter att hela sidans innehåll visats på webbplatsen.

3. En mening skrivs om vilken förbättringspotential som finns på sidan.

4. Resultaten sammanfattas i en analys där de vanligaste förbättringsåtgärderna noteras.

5. Webbplatserna rangordnas utifrån de mätningar som gjorts.


Material
-----------------------
LePage (2014, uppdaterad 2020) beskriver att bilder ofta det kräver mest utrymme vid nedladdning av en webbplats. 60% av det som laddas vid visande av en webbplats upptas av bilder. Vidare beskriver han fyra tips för att kombinera optimering och användarupplevelsen vid inladdning av bilder. De fyra delar han nämner är; användande av relativ bildstorlek, picture-element, srcset och x i img-element (för att välja rätt pixel-densitet för användare) samt användande av inline-images för att minska antalet anrop på filer. Ett exempel på det sistnämnda är svg-filer som kan skrivas inline.

Webbplatsen MOZ (https://moz.com/learn/seo/page-speed) beskriver vad page speed är och hur man kan reducera laddningstider. Följande är delar som omnämns minska laddningstider:
* Möjliggöra att filer kan komprimeras.
* Minifiering av Html-, Css- och JavaScript-filer optimerar sidan genom att ta bort onödig information i filerna.
* Ett minskat antal requests internt på webbplatsen.
* Borttagande av onödiga script-block med Javascript i html-elementet.
* Optimera serverns responstid.
* Användande av CDNs (content delivery networks), för att användare ska få snabbare och bättre tillgång till webbplatsen.
* Optimera bilder, genom att använda rätt typ av filer. Jpg, eller jpeg, är bäst för fotografier medan png beskrivs vara bra för grafik.

Verktyget PageSpeed beskrivs mäta en rad parametrar kopplade till en webbplats prestanda. Den parameter som dokumenterats i resultatet är webbplatsen prestanda (performance).

Resultat
-----------------------
*Förklaringar kopplat till förkortningar i kalkylbladet:*
*FCP - First Contentful Paint, TTI - Time to Interactive, SI - Speed Index, TBT - Total Blocking Time, LCP - Largest Contentful Paint, CLS - Cumulative Layout Shift*

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
Det har varit intressant att använda verktyget PageSpeed i uppgiften. Det är också intressant att jämföra resultaten från PageSpeed med de mätvärden som hämtades från dev-tools. Moz-artikeln tar upp flera av de förbättringsmöjligheter som PageSpeed-mätningarna genererat. Att reducera mängden oanvänd Javascript i kombination med att minska andelen innehåll som blockerar sidans rendering, verkar vara de främsta förbättringsmöjligheterna avseende de tre sidor som ingår i mätningarna. Bildhanteringen förefaller, med undantag från Sketch, vara bra.

Det som stack ut i prestandamätningarna var att Adobe fick förhållandevis låga poäng i mobil-versionen. Tittar man på resultatet så ser man att sidans laddningstider är långa avseende allt utom FCP (first contentful paint) och LCP (largest contentful paint). Siffrorna för Adobe är något bättre i desktop-versionen. Jämför man med Adobes resultat för laddade resurser ser man å andra sidan att sidan har bäst resultat avseende både antalet laddade resurser, laddningstid och storlek. Detta skulle möjligen kunna förklaras av hur mätningen är gjord och valet av värden som gjorts från dev-tools. Det är dock även en möjlighet att Adobes prestanda påverkas av att de har innehåll som blockerar sidans rendering. I sådant fall skulle borttagande av innehåll som blockerar sidans rendering möjligen ha positiv effekt på sidans prestandapoäng.

Referenser
-----------------------
LePage, Pete. 2014 (uppdaterad 2020). *https://web.dev/responsive-images/*. Läst 2022-11-18.

*https://moz.com/learn/seo/page-speed*. Läst 2022-11-18.




Övrigt
-----------------------


Författare: anjc20
