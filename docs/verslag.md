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

Op de arbeidsmarkt is er veel vraag naar front-enddevelopers die een front-endframework zoals React, Vue en/of Svelte beheersen. GSAP is een vaardigheid die ik in combinatie met een van deze frameworks kan inzetten. Dit kan mij helpen om mezelf op de arbeidsmarkt te bewijzen en mijn kennis van JavaScript en later ook React verder te ontwikkelen.

### Onderbouwing onderzoek en keuze

Ik kies uiteindelijk voor GSAP, omdat het veel flexibiliteit doordat het de optie geeft om zelf animatie delen geeft. Ook omdat het veel wordt gebruikt, is er naast de documentatie ook veel informatie beschikbaar. De mogelijkheid om GSAP met verschillende front-endframeworks, zoals Svelte en React, te gebruiken, maakt het een populaire keuze voor veel bedrijven [^6]. Dankzij de eenvoudige en uitgebreide 'Install Helper' is het bovendien makkelijk om een nieuw project te starten [^6].

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

Een duidelijk, uitgebreid prototypevoorstel dat past bij de gestelde leerdoelen.

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

### mijn idee voor een portfolio website 

het grootte idee: Een portfolio website heeft het doel om mij als persoon te laten zien aan de arbeidsmarkt en de wereld. Dit moet laten zien wat mijn skills zijn en actergrond. 

Maar wat wil ik laten zien? Ik kijk en speel veel media dust het zou mij luek lijken om dat bij mijn portfolio kunnen toevoegen.

hero/top van de site: bovenaan wil ik insiratie nemen van mijn eerste stuk media "Project moon" speciefiek "limbus company" en zijn UI. Ik wil een mechanische gevoel een uitterlijk geven aan de UI en stijfe animaties gebruiken die dat meegeven.

als je de website opent stel ik mij voor dat een mechanische arm een scherm binnen in het midden of de zijkant van van het scherm. Hierop komen dan willekeurig letters te verschijnen die constant veranderen tot dat ze komen te stoppen op mijn naam. Ik denk dat ik wel de foto eruit laat niet omdat ik mijn gezicht niet wil laten zien meer om niet van de gebruikers ervaring weg te nemen.

eronder als ik projecten wil laten zien wat ik mezelf voorstel zijn kaarten die de gebruiken kan rond dragen met een arm dat die kaart omhoog houd. als de kaart verplaatst wordt gaat de arm weg en komt het terug op de plek waar de kaart is om het omhoog te houden. 

voor verder in de website wil ik een tijdlijn waarbij je horizontaal kan scrollen om de volledige tijdlijn te kunnen zien. 

om mijn skills te laten zien wil ik deze laten binnen zweven of bewegen via een arm terwijl je scrollt. 

bij de footer wil ik een herhalende animatie die enige laatste dingen laat zien en ook een interactive contact section of pagina

voor de navbar wil ik dat het vanuit buiten het scherm komt mechanische of niet het moet een lueke animatie en niet statisch zijn. ik kan het laten verschijnen met een hover luisteraar aan de bovekant van de pagina.



### Planning

Maak een planning met een uitgewerkte tijdslijn van de te volgen stappen om je leerdoelen te behalen. Neem hierin ook de tijd op die je nodig hebt om je prototype te maken.

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