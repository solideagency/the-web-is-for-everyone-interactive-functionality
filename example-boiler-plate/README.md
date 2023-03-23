# Content Layer WTF?!

## Grote plaatje schetsen: refactor + resimpel

In deze les ga ik vanaf nul de basisfunctionaliteit nabouwen n.a.v. het voorbeeld van Justus. Hoe werkt het? Wat betekent het? Wat doet het? Ik ga jullie laten zien hoe je kan ontdekken en begrijpen door te gaan 'pielen'. Lekker spelen!

## Opzet project

- NPM init + npm install ejs express
- Package.json aanpassen: start script
- index.js boiler plate doorlopen
- app starten en testen
- Package.json aanpassen: module, start script

### Wat gaan we maken?

- Voorbeeld laten zien, waar willen we naar toe
- eerste route bepalen voor de homepagina: get('/')

### get('/')

- reponse.render, views mapje aanmaken, index.ejs en
- bepalen welke data we nodig hebben en hoe krijgen we die terug van de API: https://whois.fdnd.nl/docs (RTFM)
- variablen aanmaken: baseurl, slug, url
- hoe komen we te weten wat de slug is? Query! Console loggen van request. Er zijn ook params..
- fetch functie gebruiken en data meesturen naar EJS
- EJS template aanpassen

### get('/new')

- EJS template aanmaken
  - method (zowel POST als GET laten zien) en action uitleggen en de basis opzetten van de post('/new')
  - zie vorig college voor semantics (zie: https://codepen.io/solideagency/pen/JjZLyOQ?editors=1000)
  - attributen die de gebruiker helpen (meer info: https://adactio.com/journal/19842)
  - optional: select maken voor de squads

### post('/new')

- postJSON functie kopieëren
- post requesten = iets meesturen, dit zit in de body
- de fetch met baseurl+url params meesturen
- ID wordt gemaakt door de API
- checken of de post is gelukt. Ja: terug naar homepagina. Nee: message bij het formulier tonen + ingevulde velden overnemen

### optimaliseren

SS:

- maak schetsen hoe jij de gebruiker wilt informeren
- db connectie mist
- posten wel/niet gelukt (meerdere manieren mogelijk, wat werkt?)

HTML:

- required
- slug check: voldoet het aan de eisen

Refactoren code:

- helpers mapje aanmaken
