# Content Layer WTF?!

## Grote plaatje schetsen: refactor + resimpel

In deze les ga ik vanaf nul de basisfunctionaliteit nabouwen wat Justus heeft voorgedaan. Hoe werkt het? Wat betekent het? Wat doet het? Ik ga jullie laten zien hoe je kan ontdekken en begrijpen door te gaan 'pielen'. Lekker spelen!

## Opzet project

- NPM init + npm install ejs express dotenv
- Package.json aanpassen: module, start script
- index.js aanmaken: express, server, views, dotenv
- routes bepalen: get('/'), get('/new'), post('/new')

### get('/')

- uitleggen hoe het zit met params en query
- EJS templates klaarzetten, fetch functie kopiëeren

### get('/new')

- EJS template aanmaken
  - method (zowel post als get laten zien) en action uitleggen en de basis opzetten van de post('/new')
  - zie vorig college voor semantics
  - attributen die de gebruiker helpen (zie artikel Krijn)
  - select maken voor de squads

### post('/new')

- postJSON functie kopieëren
- voeg de regels toe voor het afhandelen van een formulier in express (anders ben je heel lang bezig.....)
- post requesten = iets meesturen, dit zit in de body
- ID wordt gemaakt door de API

### optimaliseren

SS:

- brainstormen wat goed werkt..
- slug bestaat al
- db connectie
- posten wel/niet gelukt (meerdere manieren mogelijk, wat werkt?)

HTML:

- required
- slug check
