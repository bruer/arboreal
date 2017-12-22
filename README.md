# arboreal

## breakpoints

- 1200px
- 960px
- 720px
- 480px
- 320px
- 240px

Valet av mina breakpoints är baserade på min laptops skärmstorlek (1440px), som jag inledningsvis delade upp i tre delar med en brytpunkt vid 1/2 av skärmstorleken (720px) samt en vid 1/3 av skärmstorleken (480px). 

Brytpunkten vid 720px bidrog huvudsakligen till att navigationsmenyn - som från början låg ytterst till vänster på sidan i en vertikal riktning - hamnade under headern i en horisontell riktning. Detta för att lämna plats för sidans övriga innehåll och optimera användandet av det smalare utrymmet. Vid nästa brytpunkt (480px) ändrades främst storleken och positioneringen av elementen i headern - detta var nödvändigt eftersom elementen skulle hamna utanför sidans marginaler annars.

Jag insåg senare att jag gärna vill få sidan ännu mer responsiv genom att anpassa fontstorleken på rubriker och paragrafer utifrån olika dimensioner på sidans bredd. För att genomföra detta delade jag upp sidan i sex delar istället för tre och hade därmed nu samma brytpunkter som innan plus tre stycken nya - en vid 1200px, en vid 960px och en vid 240px - alla med ett mellanrum på 240px från varandra. Detta gav mig det utrymme jag ansåg mig behöva för att göra sidan mer responsiv.

Slutligen beslöt jag mig för att lägga till ännu en brytpunkt vid 320px för att göra så att sidan ser bra ut även i mobilformat av den mindre storleken (m.a.o. med en bredd mellan 240px och 320px). Tidigare hamnade t.ex. headern utanför sidans kanter innan den sista brytpunkten vid 240px hade nåtts.

## responsivt mönster

Jag började arbetet med utgångspunkten att jag ville göra en sida med ett avskalat innehåll där endast det absolut nödvändigaste fanns med. Utifrån det var det logiskt att välja en single page-layout då den typen är rimlig när man inte har så mycket innehåll att skapa utrymme för. Därifrån tog jag inspiration från "**Holy Grail**"-layouten, med en header som tar upp den översta delen, tre kolumner bredvid varandra placerade i mitten och en footer som tar upp den nedersta delen av sidan. Dock valde jag att minska antalet kolumner från tre till två stycken, då jag endast behövde en kolumn för navigation och den andra för sidans huvudinnehåll. 

Eftersom jag personligen nästan uteslutande besöker webbsidor på större skärmar (desktop och laptop) var det naturligt för mig att arbeta efter en desktop first-paradigm. Jag hade mycket utrymme att röra mig med i ett helskärmsläge och jag valde att fylla ut sidan genom att lägga navigationsmenyn i en kolumn till vänster, istället för att placera den som en rad högst upp vilket kanske är det mer konventionella sättet. Denna layout implementerade jag först när jag gjorde sidan responsiv i del två av arbetet; efter att pixelvärdet för sidans bredd hade blivit mindre än den mittersta brytpunkten lät jag med hjälp av media queries navigationskolumnen byta plats och riktning. Vid detta tillstånd ligger sidans komponenter staplade på varandra i en gemensam kolumn.

Den andra kolumnen (till höger om navigationen) skulle bestå av sidans huvudinnehåll, vilket var en tabell, ett formulär och i övrigt text. Alltså en simpel layout med ett fåtal element, bestående av främst rubriker och paragrafer i en enstaka kolumn - detta tillät mig att applicera det responsiva mönstret "**Tiny Tweaks**" (med vissa egna modifieringar) på denna del av sidan.  
## feedback

- **Layouten består av endast färger vilket gör att sidan ser tom ute; fler bilder kan liva upp utseendet.**

Som jag nämnde tidigare var det ett medvetet val att göra min sida så stilren och avskalad som det var möjligt, då jag var rädd att det skulle se plottrigt och ogenomtänkt ut med en massor av bilder. Jag saknar tidigare erfarenhet inom webbdesign och ville helt enkelt inte ge mig in på för djupt vatten. Självklart är det helt klart genomförbart att ha med t.ex. bilder och samtidigt ha ett en stilren layout i övrigt - men jag saknade helt enkelt den kunskap och tid det skulle krävas för att implementera detta på ett sätt jag var nöjd med.

Mitt mål under arbetet var att lägga in passande bilder men väldigt mycket tid gick åt att bara få det lilla innehållet jag redan hade att fungera bra responsivt. Detta gjorde att jag tillslut övergav den ursprungliga planen.

- **Svårt att läsa CSS-koden; kommentarer skulle behövas.**

Detta håller jag med om till 100 procent då jag är en nybörjare på CSS. Jag har därför försökt att förklara CSS-dokumentet med kommentarer.

- **Sidan är inte responsiv; den skalar inte bra mot olika skärmstorlekar. Avsaknaden av flex-wrap i CSS-koden bidrar till detta.**

Detta var också helt sant och jag ägnade därför majoriteten av andra delen av arbetet åt att få sidan responsiv. Jag lyckades dock ofta lösa detta med andra metoder än med specifikt flex wrap (förutom vid ett tillfälle där jag ville få min tabell responsiv).

## W3C HTML Validator output:

Document checking completed. No errors or warnings to show.

Used the HTML parser.

Total execution time 143 milliseconds.

<p>
    <a href="https://imgur.com/buZ8HV2">
        <img src="https://i.imgur.com/buZ8HV2.png" title="source: imgur.com" />
    </a>
</p>


## W3C CSS Validator output:

Congratulations! No Error Found.
This document validates as CSS level 3 !

<p>
    <a href="http://jigsaw.w3.org/css-validator/check/referer">
        <img style="border:0;width:88px;height:31px"
            src="http://jigsaw.w3.org/css-validator/images/vcss"
            alt="Valid CSS!" />
    </a>
</p>

<p>
    <a href="https://imgur.com/11kKVak">
        <img src="https://i.imgur.com/11kKVak.png" title="source: imgur.com" />
    </a>
</p>

<p>
    <a href="https://imgur.com/cvJbOtW">
        <img src="https://i.imgur.com/cvJbOtW.png" title="source: imgur.com" />
    </a>
</p>
