# Titel verslag

Versienummer: 1

Auteur: Bram Hooiveld

Studentnummer: 0266808

Klas: 24SDB

Naam keuzedeel: Verdieping Software

Code keuzedeel:

Datum: 16-9-2026

---

<div style="page-break-after: always;"></div>

## Inhoudsopgave

- [Titel verslag](#titel-verslag)
    - [Inhoudsopgave](#inhoudsopgave)
    - [Inleiding](#inleiding)
    - [Maakt een keuze voor software](#maakt-een-keuze-voor-software)
        - [Onderzoek](#onderzoek)
        - [Vergelijking](#vergelijking)
        - [Keuze](#keuze)
        - [Arbeidsmarkt](#arbeidsmarkt)
        - [Onderbouwing onderzoek en keuze](#onderbouwing-onderzoek-en-keuze)
    - [Bronnen](#bronnen)

<div style="page-break-after: always;"></div>

## Inleiding

Op woensdag 16 september is het keuzedeel Verdieping Software begonnen. Hierbij moeten we kiezen waarin we ons de komende 20 weken of minder willen verdiepen. Ik maak hierbij mijn keuze voor de software die ik wil gebruiken. Ik kies drie opties uit de gekozen categorie en onderzoek deze. Na mijn onderzoek maak ik mijn definitieve keuze waarin ik mij wil verdiepen.

## Maakt een keuze voor software

Voor het keuzedeel wil ik mij verdiepen in JavaScript. Niet alleen in JS zelf, maar ook in een JS-library die zich richt op het animeren van elementen op een website.

### Onderzoek

Voor het onderzoek heb ik drie libraries gevonden. Voor elke library bekijk ik de websites waarop deze wordt gebruikt, evenals de documentatie en demo's, als die er zijn. Ik ga niet zoeken naar vacatures voor elke library, omdat er niet specifiek naar één library wordt gevraagd.

De libraries die ik heb gekozen om te onderzoeken zijn:

- GSAP
- Anime.js
- Motion.dev (heette eerst Framer Motion)

### [GSAP](https://gsap.com/)

GSAP is een van de meest populaire JavaScript-animatielibraries. De library wordt onder andere gebruikt door [YouTube](https://www.youtube.com/), [Netlify](https://www.netlify.com/) en [EA](https://www.ea.com/) [^6].

Het opstarten van GSAP

GSAP kan op verschillende manieren in je project worden geïmporteerd.

- Een npm- of yarn-commando
- Een CDN-link

Ook kun je een lijst met functionaliteiten invullen om automatisch een lijst met imports te krijgen [^6].

```JS
gsap.to(".box", { x: 200 })
```

Om een box te animeren, gebruik je een methode van het object `gsap`, gevolgd door de juiste class of id van het HTML-element tussen aanhalingstekens. Het gedeelte tussen `{}` geeft aan wat we ermee willen doen. In dit voorbeeld beweegt het blok 200 px over de x-as.

### [Anime.js](https://animejs.com/)

Anime.js is net als GSAP een JavaScript-animatielibrary. Anime.js kan worden gebruikt met JavaScript en React. De library wordt gebruikt door [Monkeytype](https://monkeytype.com/) en in reclames op [TikTok](https://ads.tiktok.com/business/en?tt4b_lang_redirect=1). Ook wordt de library gebruikt door [Riverside](https://riverside.com/) [^9].

Het opstarten van Anime.js

- Met npm
- Met een CDN
- Door de library rechtstreeks uit de repository te downloaden

Anime.js heeft ook uitgebreide documentatie over de verschillende manieren waarop je de library kunt gebruiken [^7].

### [Motion.dev](https://motion.dev/)

Motion.dev is een flexibele JS-library die je kunt gebruiken met JS, React, Vue, Three.js en WebGPU. De library heeft ook ontwikkeltools, zoals een AI-kit, CSS Studio en MotionScore [^5]. Motion.dev heeft veel partners [^8], zoals [Figma](https://www.figma.com/), [Linear](https://linear.app/) en [Sanity](https://www.sanity.io/).

Het opstarten van Motion.dev

- Met een packagemanager zoals npm of yarn
- Met een scripttag in de HTML

Het gebruiken van Motion [^5]:
Importeer de animatiefunctie:

```JS
import { animate } from "motion"
```

Gebruik `animate()` met een CSS-selector of met het element zelf.

```JS
// CSS selector
animate(".box", { rotate: 360 })

// Elements
const boxes = document.querySelectorAll(".box")

animate(boxes, { rotate: 360 })
```

### Vergelijking

|         | Anime.js | GSAP |  Motion.dev |
| :-------------- | :--------------: | :-----------: | :---------: |
| **Prestatie**  | Lichtgewicht en geschikt voor diverse webanimaties zonder plugins [^1]| Geschikt voor snelle en geavanceerde animaties dankzij de vele plugins. Met lagSmoothing kun je problemen door CPU-pieken helpen voorkomen. Er zijn ook veel optimalisaties beschikbaar [^4] [^6] [^10] [^11]| Gemaakt voor moderne en vloeiende animaties in de browser [^5]  |
| **Functies** | Biedt de mogelijkheid om CSS, versleepbare elementen, SVG, scrollobservatie en staggering te gebruiken. Je kunt de library gebruiken met JavaScript en React [^7].  | GSAP biedt veel mogelijkheden. Je kunt het gebruiken met vanilla JS, React, Svelte, Vue en meer, zoals WebGL, Three.js en Webflow [^6].| Motion.dev heeft uitgebreide documentatie en kan worden gebruikt met frameworks zoals React en Vue, maar ook met vanilla JavaScript [^5] |
| **Gemak van gebruik** | Anime.js is een flexibele JavaScript-library voor het maken van webanimaties. Je kunt de library met npm of via een CDN in een project gebruiken [^7]. | GSAP heeft een uitgebreide 'Install Helper' waarmee je de library eenvoudig met npm, yarn of een CDN kunt installeren. Je kunt ook eenvoudig plugins en extra toevoegingen selecteren om de bijbehorende imports te krijgen [^6]. | Redelijk gemakkelijk en goed te gebruiken met React. De library kan worden geïnstalleerd met npm of via een scripttag [^5].                         |
| **Grootte** |  Anime.js bestaat uit veel kleine bestanden, waarvan er veel kleiner zijn dan 10 kilobytes [^7]. Je importeert alleen wat je nodig hebt. |  De library is groter dan andere, vooral met extra plugins. |  De library is flexibel: je hoeft alleen te importeren wat nodig is voor jouw project [^5]. |
| **Ecosysteem** | Goede documentatie en een gemeenschap, maar kleiner dan die van grotere animatielibraries [^7] [^4]  |   GSAP heeft een groot gebruikersbestand en wordt door veel bedrijven gebruikt. De library heeft ook veel maandelijkse downloads [^4]. Daarnaast is er buiten de officiële website veel informatie te vinden [^2] [^3] [^6]. | Het is een bekende library met uitgebreide documentatie voor JavaScript, React en Vue. Ook wordt de library door bekende bedrijven gebruikt [^8] [^5]. |

### Keuze
Uit de drie JavaScript-libraries kies ik voor GSAP.

### Arbeidsmarkt
Voor front-endfuncties waarbij interactieve animaties op websites worden gemaakt, is GSAP een goeie aanvulling op JavaScript en een framework zoals React. De library wordt door verschillende bekende bedrijven gebruikt [^6], dus ervaring met GSAP kan aansluiten bij technieken die in professionele projecten worden ingezet. Door GSAP met React te combineren, kan ik laten zien dat ik niet alleen een framework beheers, maar ook complexe en vloeiende animaties kan bouwen. Zo kan ik mijn front-endvaardigheden verder ontwikkelen en mij met deze specifieke combinatie onderscheiden op de arbeidsmarkt.

### Onderbouwing onderzoek en keuze
Ik kies uiteindelijk voor GSAP, omdat het veel flexibiliteit heeft. Ook omdat het veel wordt gebruikt, is er naast de documentatie ook veel informatie beschikbaar. De mogelijkheid om GSAP met verschillende front-endframeworks, zoals Svelte en React, te gebruiken, maakt het een populaire keuze voor veel bedrijven [^6]. Dankzij de eenvoudige en uitgebreide 'Install Helper' is het bovendien makkelijk om een nieuw project te starten [^6].

---

## Maakt zich de software eigen

### Reflectie

Wat weet je al, wat weet je nog niet en wat wil je nog leren? Maak een overzicht van wat je al weet, wat je nog niet weet en wat je nog wilt leren. Zo krijg je inzicht in wat je al weet, en dus ook weet wat je nog niet weet. Neem de tijd om hierop te reflecteren.

S.
Tijdens het onderzoek heb ik veel voorbeelden gevonden van websites die de JS-libraries gebruiken, zoals Figma, Motion, Monkeytype, Anime.js, YouTube en GSAP. Hoewel ik websites en praktische voorbeelden kon vinden, kon ik geen vacatures vinden waarin specifiek naar deze JavaScript-libraries werd gevraagd. Het dichtstbij kwam ik bij vacatures voor front-enddevelopers die een framework zoals React beheersen, in combinatie waarmee ik GSAP kan gebruiken.

T.
Mijn taak was om drie softwarebibliotheken op vijf punten te vergelijken binnen de gekozen categorie, in dit geval JavaScript-animatiebibliotheken. Ik heb geen directe vacatures gevonden, maar wel genoeg websites die deze libraries gebruiken.

A.
Om zoveel mogelijk over elke library te weten te komen, heb ik websites geraadpleegd die de populariteit van de libraries met elkaar vergelijken. Ook heb ik de websites van de libraries zelf bekeken. Daar kon ik de meeste informatie vinden, zoals welke websites de libraries gebruiken.

R.
Aan het einde van mijn onderzoek heb ik de drie libraries met elkaar vergeleken en mijn keuze gemaakt. Ik heb uiteindelijk voor GSAP gekozen.

R.
Ik kon snel drie libraries vinden, maar het was lastig om veel informatie over hun relevantie op de arbeidsmarkt te vinden. Ik vond het onderzoek wel inspirerend. In eerste instantie dacht ik dat Anime.js mijn eerste keuze zou zijn. Na meer onderzoek bleek GSAP beter aan te sluiten bij wat ik wilde leren en kwam ik erachter dat het veel wordt gebruikt.

### Leerdoelen formuleren

Maak een overzicht van je leerdoelen. Wat wil je leren en wat wil je bereiken? Formuleer je leerdoelen [SMART](https://www.uu.nl/sites/default/files/upper_leerdoelen_smart_opstellen.pdf).

Aan het einde wil ik deze drie dingen hebben geleerd:
- hoe ik een of meerdere elementen kan animeren
- hoe ik met scrollen kan animeren
- hoe ik complexe animaties kan opbouwen en beheersen met timelines  

#### 1. een of meerdere elementen kunnen animeren
ik één of meerdere elementen kunnen animeren, zoals knoppen, achtergrondselementen en modals. Ik wil minimaal drie elementen kunnen animeren, de animatie kunnen laten herhalen en ervoor zorgen dat elementen kunnen reageren op gebruikersinvoer. Dit moet ik doen in een praktische applicatie en het moet gebruiksvriendelijk zijn voor de gebruiker. Dit doel helpt mij bij het leren van de basis, zodat ik dit later altijd kan gebruiken en niet slechts één keer en daarna nooit meer. ik dit in week 46 tussen 11 en 13 November mee bezig.

#### 2. hoe ik met scrollen kan animeren
Ik wil met GSAP de website kunnen laten reageren op het scrollgedrag van de gebruiker, zodat animaties kunnen worden geactiveerd en afgespeeld wanneer elementen zichtbaar worden in de viewport. Hiervoor wil ik, met behulp van de documentatie en andere bronnen, twee animaties maken die reageren op zichtbaarheid in de viewport. Dit helpt mij om een essentieel onderdeel van GSAP te leren en mijn kennis op dit gebied uit te breiden. Dit doel is haalbaar omdat het een basisonderdeel van GSAP is en niet bijzonder complex is. Ik wil dit leren in week 47 tussen 18 en 20 November.

#### 3. hoe ik complexe animaties kan opbouwen en beheersen met timelines 
Ik wil met GSAP-timelines complexe animaties kunnen opbouwen en beheersen, waarbij ik meerdere animaties combineer en de timing en volgorde nauwkeurig afstem om vloeiende overgangen te creëren. Hiervoor wil ik, met behulp van de documentatie en andere bronnen, minstens één interactieve webanimatie ontwikkelen waarin verschillende elementen samen of na elkaar bewegen. Dit helpt mij om mijn kennis van GSAP-timelines uit te breiden en te leren hoe ik meerdere animaties op een samenhangende en gebruiksvriendelijke manier kan combineren. Dit doel is haalbaar omdat ik hiermee voortbouw op mijn eerdere kennis van GSAP en stap voor stap complexere animaties leer maken. Ik wil dit doel tegen het einde van mijn project bereiken. Ik wil dit leren in week 48 tussen 25 en 27 November


### Prototype voorstel

In het stuk hieronder brainstorm ik wat ik wil maken en hoe mijn denk process verloopt.

Ideën:
Portfolio?
Informatief?
Showcase?

**PORTFOLIO**
Ik weet niet wat het meest passend zou zijn om het te leren. Een portfolio zou mij helpen met mezelf naar voren te brengen, maar kan veel tijd nemen. 

**INFORMATIEF**
Voor de informatieve website zou mij leren om de website levend te laten voelen, maar ik kan beter het statisch om een betere leeservaring. Het beste wat ik ervan kan maken, is een interactieve website met veel animaties die reageren op de user.

**SHOWCASE**
Een showcase zou inhouden dat ik mijn skills over het kuezedeel laat zien. Maar hoe doe ik dat? Ik moet er dan vanuit gaan dat ik genoeg testprojecten (klein of groot) heb om te laten zien. Maar dit kan ook beter bij een portfolio.

**BLIJVEN VRAGEN**
Showcase zou niet werken in zijn eentje, dus die combineer ik met portfolio. Informatief is een beetje groot en uitgerbreid hoe zou ik dit kunnen verkleinen? 

Wat voor informatie wil ik laten zien? wil ik alleen één ding laten zien of wil ik meerdere dingen? is het primair alleen text of zijn er ook foto's? Hoe wil ik deze informatie laten zien? 

Maar wil ik een portfolio maken. Hoe zou het in mijn voordeel zij? Zou het te veel kunnen zijn voor mij om te maken? 

De project voor het kuezedeel kan niet te persoonlijk zijn of moet het? moet het resultaat alleen persoonlijk een stap verder brengen of ook in mijn educatie. Zowiezo brengt het me een stap verder want dan heb ik alle drie benodigde keuzedelen gemaakt. En of ik een portfolio of een informatieve website maak het beide leren mijn hoe ik GSAP kan gebruiken. 

Moet ik een website hebben waar de animaties voorop staan of wat meer in de achtergrond? 

Een portfolio website is al informatief en ik heb nog geen portfolio dus ik kan deze kans te nemen terwijl ik leer om een portfolio te maken en ernaa te verberten als nodig. 

### Mijn idee voor een portfoliowebsite

Ik kijk en speel graag verschillende soorten media. Het lijkt me leuk om die interesse terug te laten komen in mijn portfolio, zonder dat de website daardoor de aandacht afleidt van mijn werk. Daarom wil ik een portfolio maken met een mechanische uitstraling en animaties die passen bij die stijl.

#### Visuele stijl

Voor de vormgeving wil ik me laten inspireren door Project Moon, en specifiek door de interface van *Limbus Company*. Ik wil een mechanisch uiterlijk combineren met strakke, stevige animaties. Zo krijgt de website een herkenbare stijl die aansluit bij mijn inspiratiebron.

#### Onderdelen van de website

- **Introductie:** Wanneer iemand de website opent, verschijnt er een mechanische arm met een scherm in het midden of aan de zijkant. Op het scherm veranderen willekeurige letters totdat mijn naam verschijnt. Ik wil geen foto van mezelf toevoegen, zodat het niet op zijn plaats uitziet.

- **Navigatie:** De navigatiebalk moet niet statisch zijn. Ik wil dat de navbar van boven of de zijkant van het scherm komt met een robotische beweging. Dit wil ik activeren met een knopje of door de gebruiker met zijn muis over een bepaald veld te zweven.

- **Tijdlijn:** Verderop wil ik een tijdlijn opnemen die bezoekers horizontaal kunnen scrollen om de volledige tijdlijn te bekijken. hier wil ik mijn ervaringen over school en het werk dat ik doe of heb gedaan. 

- **Vaardigheden:** Ik wil mijn vaardigheden willen laten zien met een herhalende animatie. Deze animatie is een carrousel die ik kan wijzigen zodat ik later terwijl ik meer skills leer ik het kan uitbreiden.

- **Projecten:** Mijn projecten wil ik presenteren als kaarten die door een mechanische arm worden vastgehouden. Wanneer een bezoeker een kaart verplaatst, beweegt de arm mee en houdt die de kaart op de nieuwe plek vast.

- **Contact en afsluiting:** Onderaan de website wil ik een herhalende animatie gebruiken om de pagina af te sluiten. Ook wil ik daar een interactieve contactsectie of contactpagina aanbieden.

### Planning

| Wanneer | Leerdoel/fase | Wat ik wil doen | Resultaat en controle |
| :-------: | :---------: | :-----------: | :-----: |
| Woensdag 11 t/m 12 november (week 46) | Leerdoel 1: basisanimaties | Ik creëer een project en bestudeer de GSAP-documentatie om de basis te leren, zoals `gsap.to()` en andere functies uit de documentatie. | Het project start en minimaal één element beweegt met GSAP. |
| Vrijdag 13 november | Het ontwerpen van mijn portfolio | Ik ga een start maken met het ontwerp van mijn portfolio. | Ik heb een lay-out voor de homepage voor desktop en mobiel. |
| Woensdag 18 t/m donderdag 19 november (week 47) | Leerdoel 2: scrollanimaties | Ik ga de documentatie van GSAP over scrollanimaties bestuderen en een keuze maken hoeveel elementen ik hiermee wil animeren. | Er zijn ten minste twee elementen die met scrollanimaties bewegen. |
| Vrijdag 20 november (week 47) | Het verder ontwerpen van mijn portfolio | Ik ga verder met het ontwerpen van mijn portfolio, zodat ik een beeld heb van wat ik wil maken. | Ik heb de lay-out gebruikt om een concreet ontwerp in Figma te maken. |
| Woensdag 25 november (week 48) | Mijn portfolio-ontwerp afmaken | Ik ga verder met het ontwerp om het af te krijgen, zodat ik het kan maken. | Het ontwerp is af voor zowel mobiel als desktop. |
| Donderdag 26 t/m vrijdag 27 november (week 48) | Leerdoel 3: tijdlijnen | Ik wil met één onderdeel meerdere elementen kunnen animeren, of hetzelfde element in een sequentie, zodat ik één lange animatie kan maken. | Er staat een eerste tijdlijn waarin meerdere elementen na elkaar of tegelijk bewegen. |
| 2 december (week 49) | Het ontwerp afmaken | Ik wil mijn ontwerp af hebben, zodat ik aan de portfolio zelf kan werken. | Een volledig ontwerp met een mobiele versie. |
| 3 t/m 4 december (week 49) | Werken aan de hero | Ik wil de hero voor mijn portfoliowebsite maken. | De hero is af. |
| 9 t/m 11 december (week 50) | De tijdlijn maken | Ik wil een duidelijke tijdlijn maken waarin ik mijn groei door de jaren heen laat zien. | Een eerste versie van de tijdlijn. |
| 16 december (week 51) | Vaardigheden | Ik wil mijn vaardigheden laten zien, zoals ik in het leerdoel heb beschreven. | Mijn vaardigheden zijn af. |
| 17 t/m 19 december (week 51) | Projectenoverzicht | Ik wil het projectenoverzicht van mijn portfolio maken, zoals ik in het voorstel heb beschreven. | Het projectenoverzicht is af en ik lig op schema om het na de vakantie op tijd af te krijgen. |
| 6 t/m 9 januari (week 1) | Mijn portfolio afmaken | Ik wil de contactsectie maken en mijn portfolio afronden. | De contactsectie en de volledige portfoliowebsite zijn af. |

### Logboek

Houd een logboek bij van de tijd die je besteedt aan het maken van je prototype. Noteer hierin ook de stappen die je hebt gezet om je leerdoelen te behalen.

## Prototype

Leg uit wat je prototype is en hoe je dit hebt gemaakt. Voeg ook een link naar je video van je prototype.

## Eindconclusie

Leerdoelen behaald? Wat heb je geleerd? Wat zou je een volgende keer anders doen? Wat zijn je vervolgstappen? 

<div style="page-break-after: always;"></div>

## Bronnen

[^1]: [annnimate.com](https://annnimate.com/compare/best-animation-libraries) door Good Fella. "Best Animation Libraries", laatst gewijzigd op 20 juli 2026.

[^2]: [wmtips.com](https://www.wmtips.com/technologies/javascript-libraries/filter/animation/). "JS libraries, most popular by 2026", de opgenomen data is laatst bijgewerkt op 28 september 2026.

[^3]: [jstool.gitlab](https://jstool.gitlab.io/blog/posts/the-most-popular-javascript-libraries-in-2026/). "The Top 100 Open-Source JavaScript Libraries", geraadpleegd op 28 september 2026.

[^4]: [bestofjs.com](https://bestofjs.org/projects?tags=animation). "Animation libraries", geraadpleegd op 28 september 2026.

[^5]: [Motion.dev](https://motion.dev/). Eerst bekend als Framer Motion. Geraadpleegd op 16 september 2026.

[^6]: [GSAP.com](https://gsap.com/). Geraadpleegd op 16 september 2026. Bijna onderaan de pagina, boven de demo's, staat welke merken GSAP hebben gebruikt.

[^7]: [Anime.js](https://animejs.com/), geraadpleegd op 16 september 2026.

[^8]: [Motion.dev partners](https://motion.dev/partners#partners). Dit zijn de partners en bedrijven waarmee Motion.dev heeft gewerkt. Geraadpleegd op 28 september 2026.

[^9]: [Wappalyzer](https://www.wappalyzer.com/technologies/javascript-graphics/anime-js/). "Websites using Anime.js", geraadpleegd op 30 september 2026. Een lijst met websites die Anime.js gebruiken.

[^10]: [annnimate.com](https://annnimate.com/compare/gsap-vs-anime-js). "Comparison between Anime.js and GSAP", geraadpleegd op 30 september 2026. Een vergelijking van GSAP en Anime.js.

[^11]: [Why GSAP](https://gsap.com/blog/why-gsap/). "FAQ for GSAP". Veelgestelde vragen over GSAP, zoals de bestandsgrootte en animaties.

##