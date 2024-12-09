---
Title: Load
Description: This is my load analysis page.
Template: analysis
---

Laddningstid
=======================

Undersöka laddningstiden och förbättringspotential på tre olika webbplatser.

Urval
-----------------------

Jag har valt följande webbplatser:

- https://www.norrmejerier.se/
- https://www.arla.se/
- https://www.skanemejerier.se/

Jag valde webbplatser från tre företag inom samma kategori: mejeri. Jag valde just dessa webbplatser för jag tycker det är intressant att jämföra konkurrenter.

Metod
-----------------------

Jag använde sidan PageSpeed Insights och noterade de olika mätvärdena på varje webbplats på tre olika sidor. Sedan använde jag DevTools i Google Chrome för att mäta laddningstid, resurser och storlek under Network-fliken. Jag laddade om sidan tre gånger (ctrl + shift + r) för att få tre mätvärden per sidan, och tog snittet av mätningarna. All datan la jag in i ett excel-ark.

Resultat
-----------------------

### Google Pagespeed mätvärden

<iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vTITbr0eDegYQaxQjdehNiBPbH78fQENco99BjWnOCikQbtRpdB1LkdwFDssb04CoH6WHZTDhS4zmyB/pubhtml?gid=0&amp;single=true&amp;widget=true&amp;headers=false" class="data-table pagespeed"></iframe>

### Devtools mätvärden

<iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vTITbr0eDegYQaxQjdehNiBPbH78fQENco99BjWnOCikQbtRpdB1LkdwFDssb04CoH6WHZTDhS4zmyB/pubhtml?gid=792854&amp;single=true&amp;widget=true&amp;headers=false" class="data-table devtools"></iframe>

### Norrmejerei

![Norrmejeri](%assets_url%/img/mejeri_norr.png) {.mejeri-img}

Sidor:
- **Hem**: https://www.norrmejerier.se/
- **Produkter**: https://www.norrmejerier.se/produkter
- **Recept**: https://www.norrmejerier.se/goda-recept

**Google Pagespeed**:

| Företag    | Sida       | Enhetstyp | LCP (s) | INP (ms) | CLS  | FCP (s) | TTFB (s) |
|------------|------------|-----------|---------|----------|------|---------|----------|
| Norrmejeri | Hem        | Mobilt    | 1.6     | 112      | 0.46 | 1.5     | 1.0      |
| Norrmejeri | Hem        | Dator     | 1.4     | 35       | 0.06 | 1.4     | 0.8      |
| Norrmejeri | Produkter  | Mobilt    | 1.3     | 94       | 0.00 | 1.2     | 0.8      |
| Norrmejeri | Produkter  | Dator     | 1.2     | 34       | 0.03 | 1.0     | 0.7      |
| Norrmejeri | Recept     | Mobilt    | 1.3     | 94       | 0.00 | 1.2     | 0.8      |
| Norrmejeri | Recept     | Dator     | 1.2     | 34       | 0.03 | 1.0     | 0.7      |

**Devtools**:

| Företag    | Sida      | Resurser | Storlek (MB) | Laddningstid snitt (ms) |
|------------|-----------|----------|--------------|-------------------------|
| Norrmejeri | Hem       | 41       | 1,9          | 561,7                   |
| Norrmejeri | Produkter | 46       | 1,8          | 914,3                   |
| Norrmejeri | Recept    | 44       | 1,5          | 615                     |

Norrmejeri får ganska bra mätvärden, förutom Cumulative Layout Shift (CLS) för mobil enhetstyp, detta skulle de kunna förbättra genom att undvika stora layoutförskjutningar.


### Arla

![Arla](%assets_url%/img/mejeri_arla.png) {.mejeri-img}

Sidor:
- **Hem**: https://www.arla.se/
- **Produkter**: https://www.arla.se/produkter/
- **Recept**: https://www.arla.se/recept/

**Google Pagespeed**:

| Företag | Sida      | Enhetstyp | LCP (s) | INP (ms) | CLS   | FCP (s) | TTFB (s) |
|---------|-----------|-----------|---------|----------|-------|---------|----------|
| Arla    | Hem       | Mobilt    | 1.2     | 198      | 0     | 1.1     | 0.5      |
| Arla    | Hem       | Dator     | 1.1     | 142      | 0.03  | 0.9     | 0.4      |
| Arla    | Produkter | Mobilt    | 1.6     | 156      | 0     | 1.4     | 1.3      |
| Arla    | Produkter | Dator     | 1.7     | 108      | 0.01  | 1.3     | 1        |
| Arla    | Recept    | Mobilt    | 2.1     | 268      | 0.07  | 1       | 0.6      |
| Arla    | Recept    | Dator     | 2.2     | 183      | 0.04  | 0.9     | 0.5      |

**Devtools**:

| Nr  | Företag | Sida      | Resurser | Storlek (MB) | Laddningstid snitt (ms) |
|-----|---------|-----------|----------|--------------|-------------------------|
| 16  | Arla    | Hem       | 90       | 5,7          | 1010,7                  |
| 20  | Arla    | Produkter | 65       | 3,4          | 3573,3                  |
| 24  | Arla    | Recept    | 90       | 6,9          | 1363,3                  |

Arla skulle kunna förbättra sig genom att reducera javascript som inte används och därmed minska tiden det tar att köra javascript kod.


### Skånemejeri

![Skånemejeri](%assets_url%/img/mejeri_skane.png) {.mejeri-img}

Sidor:
- **Hem**: https://www.skanemejerier.se/
- **Produkter**: https://www.skanemejerier.se/sortiment
- **Recept**: https://www.skanemejerier.se/recept

**Google Pagespeed**:

| Företag     | Sida      | Enhetstyp | LCP (s) | INP (ms) | CLS   | FCP (s) | TTFB (s) |
|-------------|-----------|-----------|---------|----------|-------|---------|----------|
| Skånemejeri | Hem       | Mobilt    | 1.8     | 134      | 0     | 0.7     | 0.4      |
| Skånemejeri | Hem       | Dator     | 1.9     | 74       | 0     | 0.7     | 0.4      |
| Skånemejeri | Produkter | Mobilt    | 1.3     | 117      | 0     | 0.7     | 0.4      |
| Skånemejeri | Produkter | Dator     | 1.4     | 65       | 0.04  | 0.7     | 0.3      |
| Skånemejeri | Recept    | Mobilt    | 1.3     | 117      | 0     | 0.7     | 0.4      |
| Skånemejeri | Recept    | Dator     | 1.4     | 65       | 0.04  | 0.7     | 0.3      |

**Devtools**:

| Företag     | Sida      | Resurser | Storlek (MB) | Laddningstid snitt (ms) |
|-------------|-----------|----------|--------------|-------------------------|
| Skånemejeri | Hem       | 32       | 2,1          | 910                     |
| Skånemejeri | Produkter | 26       | 1,4          | 719,3                   |
| Skånemejeri | Recept    | 32       | 1,4          | 705,7                   |

Skånemejeri får bra prestanda-betyg hos Google Pagespeed, men de skulle kunna reducera javascript som inte används.

Analys
-----------------------

Vanliga förbättringsåtgärder är att minska javascript-kod som inte används, det är en varning som alla hemsidor fick. Många av sidorna använder sig av stora element, till exempel bilder, som ökar på laddningstiden rejält. Många sidor skulle även kunna använda bilder med rätt storlek för bättre databesparing.

Här har jag rangordnat sidorna utefter snitt laddningstid enligt Devtools. Norrmejeri får generellt bäst laddningstid, nästbäst är Skånemejeri och sist kommer Arla. Detta är rimligt då Arla har störst värden under "Storlek (MB)" och "Resurser"

| Företag     | Sida       | Resurser | Storlek (MB) | Laddningstid snitt (ms) |
|-------------|------------|----------|--------------|-------------------------|
| Norrmejeri  | Hem        | 41       | 1,9          | 561,7                   |
| Norrmejeri  | Recept     | 44       | 1,5          | 615                     |
| Skånemejeri | Recept     | 32       | 1,4          | 705,7                   |
| Skånemejeri | Produkter  | 26       | 1,4          | 719,3                   |
| Skånemejeri | Hem        | 32       | 2,1          | 910                     |
| Norrmejeri  | Produkter  | 46       | 1,8          | 914,3                   |
| Arla        | Hem        | 90       | 5,7          | 1010,7                  |
| Arla        | Recept     | 90       | 6,9          | 1363,3                  |
| Arla        | Produkter  | 65       | 3,4          | 3573,3                  |

Largest Contentful Paint (LCP) mäter hur lång tid det tar för största elementet att rendera, detta är alltså ett ganska viktigt mätvärde för användarupplevelsen. Här har jag rangordnat sidorna efter LCP. Vi ser att det är ganska blandat och det är svårt att hitta en klar vinnare då Arla är både först och sist. Vi kan se att Norrmejeri hamnar högt upp på nästan alla sina sidor, alltså skulle jag säga att Norrmejeri vinner. Enligt Google Pagespeed klassas allt under 2,5 sekunder som bra, 2,5 - 4 sekunder som medel och över 4 sekunder som dåligt. Det sämsta mätvärdet här är 2,2 sekunder, alltså är alla mätvärden bra.

| Företag     | Sida      | Enhetstyp | LCP (s) |
|-------------|-----------|-----------|---------|
| Arla        | Hem       | Dator     | 1,1     |
| Norrmejeri  | Produkter | Dator     | 1,2     |
| Norrmejeri  | Recept    | Dator     | 1,2     |
| Arla        | Hem       | Mobilt    | 1,2     |
| Norrmejeri  | Produkter | Mobilt    | 1,3     |
| Norrmejeri  | Recept    | Mobilt    | 1,3     |
| Skånemejeri | Produkter | Mobilt    | 1,3     |
| Skånemejeri | Recept    | Mobilt    | 1,3     |
| Norrmejeri  | Hem       | Dator     | 1,4     |
| Skånemejeri | Produkter | Dator     | 1,4     |
| Skånemejeri | Recept    | Dator     | 1,4     |
| Norrmejeri  | Hem       | Mobilt    | 1,6     |
| Arla        | Produkter | Mobilt    | 1,6     |
| Arla        | Produkter | Dator     | 1,7     |
| Skånemejeri | Hem       | Mobilt    | 1,8     |
| Skånemejeri | Hem       | Dator     | 1,9     |
| Arla        | Recept    | Mobilt    | 2,1     |
| Arla        | Recept    | Dator     | 2,2     |

Interaction to Next Paint (INP) mäter hur lång tid det tar innan man kan interagera med sidan igen efter en åtgärd. Här ser vi att Norrmejeri får bäst resultat, sen kommer Skånemejeri och sist Arla.

| Företag     | Sida      | Enhetstyp | INP (ms) |
|-------------|-----------|-----------|----------|
| Norrmejeri  | Produkter | Dator     | 34       |
| Norrmejeri  | Recept    | Dator     | 34       |
| Norrmejeri  | Hem       | Dator     | 35       |
| Skånemejeri | Produkter | Dator     | 65       |
| Skånemejeri | Recept    | Dator     | 65       |
| Skånemejeri | Hem       | Dator     | 74       |
| Norrmejeri  | Produkter | Mobilt    | 94       |
| Norrmejeri  | Recept    | Mobilt    | 94       |
| Arla        | Produkter | Dator     | 108      |
| Norrmejeri  | Hem       | Mobilt    | 112      |
| Skånemejeri | Produkter | Mobilt    | 117      |
| Skånemejeri | Recept    | Mobilt    | 117      |
| Skånemejeri | Hem       | Mobilt    | 134      |
| Arla        | Hem       | Dator     | 142      |
| Arla        | Produkter | Mobilt    | 156      |
| Arla        | Recept    | Dator     | 183      |
| Arla        | Hem       | Mobilt    | 198      |
| Arla        | Recept    | Mobilt    | 268      |

Cumulative Layout Shift (CLS) mäter hur mycket sidan rör på sig medan den laddar. Här har alla sidor värden nära 0, förutom Norrmejeris hemsida för mobila enheter, som har ett markant högre värde. Här blir Skånemejeri vinnare, sedan Arla och sist Norrmejeri.

| Företag     | Sida      | Enhetstyp | CLS  |
|-------------|-----------|-----------|------|
| Skånemejeri | Hem       | Dator     | 0    |
| Norrmejeri  | Produkter | Mobilt    | 0    |
| Norrmejeri  | Recept    | Mobilt    | 0    |
| Skånemejeri | Produkter | Mobilt    | 0    |
| Skånemejeri | Recept    | Mobilt    | 0    |
| Skånemejeri | Hem       | Mobilt    | 0    |
| Arla        | Produkter | Mobilt    | 0    |
| Arla        | Hem       | Mobilt    | 0    |
| Arla        | Produkter | Dator     | 0.01 |
| Norrmejeri  | Produkter | Dator     | 0.03 |
| Norrmejeri  | Recept    | Dator     | 0.03 |
| Arla        | Hem       | Dator     | 0.03 |
| Skånemejeri | Produkter | Dator     | 0.04 |
| Skånemejeri | Recept    | Dator     | 0.04 |
| Arla        | Recept    | Dator     | 0.04 |
| Norrmejeri  | Hem       | Dator     | 0.06 |
| Arla        | Recept    | Mobilt    | 0.07 |
| Norrmejeri  | Hem       | Mobilt    | 0.46 |

First Contentful Paint (FCP) mäter tiden det tar innan det första elementet syns på sidan, alltså hur snabbt man ser att sidan börjar ladda. Här vinner Skånemejeri, sedan kommer Arla och sist Norrmejeri.

| Företag     | Sida      | Enhetstyp | FCP (s) |
|-------------|-----------|-----------|---------|
| Skånemejeri | Hem       | Dator     | 0,7     |
| Skånemejeri | Produkter | Mobilt    | 0,7     |
| Skånemejeri | Recept    | Mobilt    | 0,7     |
| Skånemejeri | Hem       | Mobilt    | 0,7     |
| Skånemejeri | Produkter | Dator     | 0,7     |
| Skånemejeri | Recept    | Dator     | 0,7     |
| Arla        | Hem       | Dator     | 0,9     |
| Arla        | Recept    | Dator     | 0,9     |
| Norrmejeri  | Produkter | Dator     | 1       |
| Norrmejeri  | Recept    | Dator     | 1       |
| Arla        | Recept    | Mobilt    | 1       |
| Arla        | Hem       | Mobilt    | 1,1     |
| Norrmejeri  | Produkter | Mobilt    | 1,2     |
| Norrmejeri  | Recept    | Mobilt    | 1,2     |
| Arla        | Produkter | Dator     | 1,3     |
| Arla        | Produkter | Mobilt    | 1,4     |
| Norrmejeri  | Hem       | Dator     | 1,4     |
| Norrmejeri  | Hem       | Mobilt    | 1,5     |

Time To First Byte (TTFB) mäter tiden det tar för den första byte av data tas emot från servern. Här vinner Skånemejeri, sedan kommer Arla och sist Norrmejeri.

| Företag     | Sida      | Enhetstyp | TTFB (s) |
|-------------|-----------|-----------|----------|
| Skånemejeri | Hem       | Dator     | 0,4      |
| Skånemejeri | Produkter | Mobilt    | 0,4      |
| Skånemejeri | Recept    | Mobilt    | 0,4      |
| Skånemejeri | Hem       | Mobilt    | 0,4      |
| Skånemejeri | Produkter | Dator     | 0,3      |
| Skånemejeri | Recept    | Dator     | 0,3      |
| Arla        | Hem       | Dator     | 0,4      |
| Arla        | Recept    | Dator     | 0,5      |
| Norrmejeri  | Produkter | Dator     | 0,7      |
| Norrmejeri  | Recept    | Dator     | 0,7      |
| Arla        | Recept    | Mobilt    | 0,6      |
| Arla        | Hem       | Mobilt    | 0,5      |
| Norrmejeri  | Produkter | Mobilt    | 0,8      |
| Norrmejeri  | Recept    | Mobilt    | 0,8      |
| Arla        | Produkter | Dator     | 1        |
| Arla        | Produkter | Mobilt    | 1,3      |
| Norrmejeri  | Hem       | Dator     | 0,8      |
| Norrmejeri  | Hem       | Mobilt    | 1        |

De mest avgörande mätvärdena skulle jag säga är sidans laddningstid och LCP, alltså blir den slutgiltiga vinnaren Norrmejeri, som var bäst i båda de kategorierna.

Min gräns för en snabb laddningstid går vid cirka 2 sekunder. Tar det längre än så tycker jag det är lite segt. Den sida som inte klarar min gräns är Arlas produkt-sida som har över 3 sekunder enligt mina mätningar. Däremot är det inte långt ifrån gränsen, så jag skulle ändå klassa det som godkänt. Förmodligen har arla väldigt många produkter och får därmed en längre laddningstid. De andra sidorna klarar min gräns bra, alla förutom Arla har under en sekund. Jag upplever dessa sidor som snabba, och Arla som helt okej snabb.

Referenser
-----------------------

- https://pagespeed.web.dev/

Övrigt
-----------------------

Författare: Paula Frölander