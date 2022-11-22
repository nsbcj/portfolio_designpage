---
Title: Colors
icon: fas fa-paint-roller
---

Rapport - Analys av färgval
=======================

Bakgrunden till rapporten är en [uppgift](https://dbwebb.se/uppgift/utvardera-webbplatsers-fargval-och-kanslan-de-signalerar-v2) inom ramen för en design-kurs på BTH.

Enligt kravspecifikationen ska uppgiften bestå av ett urval av minst tre webbplatser, vars typografi och färgpalett ska dokumenteras. Analysen ska bestå av argumentationer kring valen av färg samt vilken känsla som webbsidorna uppfattas förmedla.

Denna rapport är skriven enskilt.

Urval
-----------------------

Urvalet är baserat på webbplatser relaterade till design. Webbplatserna innehåller bland annat verktyg som underlättar designprocesser.

Anledningen till att design-plattformars webbplatser valts, är att deras produkt rör design. Att företagen arbetar med design, bör återspeglas i valet av design på webbplatserna.

Följande är en sammanställning av urvalet:

|   Webbplats          |    Bild    |    Kontrolldatum       |
|   ---------          |    ----    |     -----      |
|   www.figma.com      | ![Bild kunde inte laddas](../image/figma.png?h=100&save-as=jpg&q=40)  |   2022-11-11  |   
|   www.adobe.com      | ![Bild kunde inte laddas](../image/adobe.png?h=100&save-as=jpg&q=40)  |   2022-11-11  |
|   www.sketch.com     | ![Bild kunde inte laddas](../image/sketch.png?h=100&save-as=jpg&q=40)  |   2022-11-11  |

Metod
-----------------------

Undersökningen har gjorts enligt kravspecifikation kopplad till uppgiften. Nedan redogörs för genomförda steg.

1. Kontroll av webbplats.
Bilder från webbplatserna har tagits med hjälp av det screenshotprogram som medföljer operativsystemet. Avgränsning har gjort till sidornas övre del, det vill säga det som syns på på sidan utan att någon scrollning genomförts.
2. Framtagande av färgpalett.
Från bilden i steg 1, har färgpalett extraherats med hjälp av Adobe Colors verktyg [Image](https://color.adobe.com/create/image). Efter att bild laddats upp i verktyget extraheras en färgpalett.
3. Noterande av färgschema och accentfärg.
Efter att färgkoderna noterats i hexadecimal, har färgkoderna kontrollerats i Adobe Colors verktyg [Color-Wheel](https://color.adobe.com/create/color-wheel). Färghjulet användes för att underlätta analysen om vilket färgschema som använts på webbplatsen.
4. Noterande av typsnitt.
Typsnittet har noterats med hjälp av dev-tools i webbläsaren. Den information som hämtats avseende typsnitten är det som framgår av informationen "font used". Specifik information om typsnitt i h1-h3 samt brödtext har hämtats genom filtrering av element i html-strukturen.
5. Notering av stil kopplad till webbplatsens syfte.
Denna del har gjorts med hjälp av referenser till kursmaterial som ingår i kursmomentet.

Sammanfattningsvis är rapporten en förenklad fallstudie av tre webbplatser. Resultatet presenteras i tabellformat, medan diskussionen utgörs av en argumentation kopplad till webbplatsernas syfte, likheter och olikheter.

Material
-----------------------
I artikeln *"An Introduction to Color Theory for Web Design"* (Cannon 2012) beskrivs kortfattat färgens betydelse inom web-design. Cannon beskriver tre delar som är av betydelse avseende färger inom design. Det är hur färger kompletterar varandra, dess kontrast och dess livfullhet.

I boken *"The Principles of Beautiful Web Design"* (Beaird, George, 2014) beskrivs bland annat vad olika färger kan representera och hur färgscheman är uppbyggda.

###Mättnad och kontrast
Beaird och George (2014) beskriver att färgens mättnad kan beskrivas som färgen styrka eller klarhet. Livliga färger sticker ut mer än färger som går mot grått eller svart.

###Analogt färgschema
Beaird och George (2014) beskriver analogt färgschema som färger som ligger intill varandra i färgshemat.

###Komplementfärg
Beaird och George (2014) beskriver i figur 2.31 att komplementfärg eller split-complementary har sin utgång i två färger intill varandra i färghjulet. Sedan väljs ytterligare en färg på motsatt sida färghjulet. Figur 2.31 visar att linjerna mellan färgerna i färghjulet formar ett smalt Y.

###Sammansatt färgschema
Cannon (2010) beskriver att ett sammansatt (compound) färgschema består av två färger valda från motsatt sida av färghjulet.

###Färgtemperatur
Beaird och George (2014) beskriver att varma färger är spektrumet från rött till gult. Färgerna representerar värme och rörelse. En annan egenskap författarna nämner är att varma färger sticker ut i kombination med kalla.

Vidare skriver författarna att kalla färger är spektrumet från grönt till blått. Dessa färger är enligt författarna lugnande och kan med fördel användas på stora element på webbplatser.   

###Betydelse av olika färger
Beaird och George (2014) beskriver associationer kopplade till färger i ett avsnitt. Färgen röd kan exempelvis associeras med kärlek, vin och höst. Orange kan förknippas med aktivitet, glädje och kreativitet. Likt orange, beskrivs gul som en aktiv färg. Grönt hänger ihop med naturen och tillväxt. Blått representerar hopp, tro, frihet och har en lugnande effekt. Blått kan även representera stabilitet. Lila har enligt författarna associerats med kunglighet och makt. Färgen uttrycker en känsla för makt och lyx. Den balanserar färgerna rött och blått. Webbplatser innehållande lila sticker enligt författarna ut.

Både vitt och svart är också färger som nämns. Vit används ofta som bakgrundsfärg. Den svarta färgen kan användas för att uttrycka makt och styrka.

Resultat
-----------------------
###www.figma.com

1. ####Färgpalett
<table style="border-spacing: 4px; border-collapse: separate">
    <tr>
        <td style="height: 50px; width: 50px; background-color: #5058F2"></td>
        <td style="height: 50px; width: 50px; background-color: #1BA0F2"></td>
        <td style="height: 50px; width: 50px; background-color: #B5F299"></td>
        <td style="height: 50px; width: 50px; background-color: #F2B90F"></td>
        <td style="height: 50px; width: 50px; background-color: #F24E1E"></td>
    </tr>
</table>

2. ####Undersökning
|   Område              | Resultat |
|   -------             |  -----   |
|   Val av färgschema   | Split complementary / Komplementfärg   |
|   Val av accentfärg   | #F2BB13 gult    |
|   Laddade typsnitt   | 2 (Whyte, DejaVu Sans)   |
|   Typsnitt h1-h3      | Whyte (primär), sans-serif (sekundär)  |
|   Typsnitt brödtext   | Whyte, sans-serif |
|   Matchande profil   | Färgvalet och typsnittet uppfattas matcha produktens/företaget profil. |  

###www.adobe.com

1. ####Färgpalett
<table style="border-spacing: 4px; border-collapse: separate">
    <tr>
        <td style="height: 50px; width: 50px; background-color: #F21D81"></td>
        <td style="height: 50px; width: 50px; background-color: #9498F2"></td>
        <td style="height: 50px; width: 50px; background-color: #D7F205"></td>
        <td style="height: 50px; width: 50px; background-color: #F2BB13"></td>
        <td style="height: 50px; width: 50px; background-color: #F20505"></td>
    </tr>
</table>

2. ####Undersökning
|   Område              | Resultat |
|   -------             |  -----   |
|   Val av färgschema   | Compound / Sammansatt    |
|   Val av accentfärg   | #216DDB blå    |
|   Laddade typsnitt   | 3 (Adobe Clean Light, Adobe Clean, DejaVu Sans)   |
|   Typsnitt h1-h3      | Adobe Clean  |
|   Typsnitt brödtext   | Adobe Clean |
|   Matchande profil   | Färgvalet och typsnittet uppfattas matcha produktens/företaget profil. |

###www.sketch.com

1. ####Färgpalett
<table style="border-spacing: 4px; border-collapse: separate">
    <tr>
        <td style="height: 50px; width: 50px; background-color: #F27F3D"></td>
        <td style="height: 50px; width: 50px; background-color: #F26430"></td>
        <td style="height: 50px; width: 50px; background-color: #F29F80"></td>
    </tr>
</table>

2. ####Undersökning
|   Område              | Resultat |
|   -------             |  -----   |
|   Val av färgschema   | Analogous / Analogt    |
|   Val av accentfärg   | #000000 svart    |
|   Laddade typsnitt   | 1 (Marfa)   |
|   Typsnitt h1-h3      | Marfa  |
|   Typsnitt brödtext   | Marfa |
|   Matchande profil   | Färgvalet uppfattas vara uttrycka något annorlunda i förhållande till de två andra sidorna. Det är i detta fall svårare att utläsa företaget/produktens profil genom att titta på färgval och typsnitt. |

Analys
-----------------------
En webbplats som sticker ut avseende färgvalet, vilket är www.sketch.com. Webbplatsen har ett färgschema som jag tror är analogt, men angränsar till monokromt. De andra webbplatserna har färgscheman som liknar varandra avseende att de använder komplementfärger. Min uppfattning är att Figma och Adobe signalerar att de arbetar med produkter som relateras till kreativitet. Sketch färgval relateras inte omedelbart till kreativitet utan snarare till en känsla av struktur.

Både Figma och Adobe kombinerar varma och kalla färger på ett intressant sätt. Beaird och George (2014) skriver att kalla färger representerar lugn och varma rörelse. De skriver också att de kalla färgerna med fördel kan användas till större element på webbplatser. Figmas webbplats är bra utformad ur detta hänseende. De kalla färgerna dominerar, samtidigt som en varm färg har valts som accent för att ringa in sidans budskap. Adobe har i sina containers använt någon form av mesh / gradients innehållande både kalla och varma färger. Kombinationen förmedlar känslan av kreativitet. Jag tror att Adobe använder färgen rött för att förmedla glädje. Beaird och George (2014) skriver att färgen lila är sällsynt i webbdesign, men jag uppfattar att färgen har en viktig roll på både Figma och Adobes webbplatser. Författarna har vidare beskrivit att svart kan användas för att uttrycka makt och styrka. Min känsla är att de som utformat Sketch webbplats har givit svart en viktig roll på webbplatsen. Den svart färgen används effektivt för att förstärka de viktiga element som visas på sidan. Den brun / orangea färgen som används på de stora elementen på Sketch webbplats, känns lite överväldigande. Kanske är det att färgen känns varm, som förstärker känslan.

En gememsam nämnare för samtliga webbplatser är att fåtal eller enstaka typsnitt används. Min uppfattning är att det förstärker känslan av att struktur och att det finns en tydlig idé med designen. En annan iakttagelse är att samtliga sidors typsnitt är sans-serif.

Referenser
-----------------------

Cannon, Thomas. 2012 *An Introduction to Color Theory for Web Design*. https://webdesign.tutsplus.com/articles/an-introduction-to-color-theory-for-web-designers--webdesign-1437. (Läst 2022-10-11).

Beaird, Jason; George, James. 2014. *The Principles of Beautiful Web Design, 3rd Edition*. Published by SitePoint.

Övrigt
-----------------------
Det uppfattades inte helt att avgöra vilka färgschema som respektive webbplats hör under, trots användandet av Adobes verktyg.

Sammanfattningsvis har det varit en intressant utmaning att analysera webbplatserna. De tre webbplatserna uppfattas ha en god design med sammanhängande färgval och typografi. Sketch förmedlar sin profil på ett annorlunda sätt en de två övriga, men uppfattas även den ha en god design.

Författare: anjc20
