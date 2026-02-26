# Introductie

MDTO staat voor **Metagegevens voor Duurzaam Toegankelijke Overheidsinformatie** en is een Nederlandse standaard voor het vastleggen van informatie over overheidsdocumenten. Het doel is om overheidsinformatie op de lange termijn vindbaar, interpreteerbaar en betrouwbaar toegankelijk te houden, ook wel duurzame digitale informatiehuishouding (DUTO) genoemd. MDTO helpt overheden bij het voldoen aan wettelijke verplichtingen en vergemakkelijkt samenwerking en gegevensuitwisseling.

## Wat is een metagegevensschema
Een metagegevensschema beschrijft de structuur, betekenis en regels waar bepaalde metagegevens aan moeten voldoen. Of zoals geformuleerd in NEN-ISO 23081 een “logische structuur die het verband aangeeft tussen elementen van metagegevens, doorgaans door regels vast te stellen voor het gebruik en beheer van metagegevens, vooral met betrekking tot de semantiek, de syntaxis en de keuzevrijheid (mate van verplichting) van waarden."

Een metagegevensschema kan voor verschillende doeleinden gebruikt worden, zoals:

- Het ontwerpen of inrichten van de metagegevensfuncties van een informatiesysteem. Een metagegevensschema beschrijft de structuur van de metagegevens. Op basis daarvan kunnen de functies voor opslag, invoeren, wijzigen en tonen van de metagegevens ontworpen worden.
- De uitleg van de betekenis van metagegevens. Bijvoorbeeld in een handleiding of als verklarende tekst in een gebruikersinterface.
- De validatie van metagegevens. Het metagegevensschema beschrijft de regels waaraan de metagegevens moeten voldoen. Op basis daarvan kunnen de metagegevens gecontroleerd worden.

## Objecten
### Soorten objecten
MDTO maakt onderscheid tussen verschillende soorten objecten waaraan metagegevens verbonden zijn:

- Informatieobject: Een op zichzelf staand geheel van gegevens met een eigen identiteit. Zoals een tekstdocument of een foto. Zie de definitie van Informatieobject voor een nadere toelichting.
- Bestand: Een geordende verzameling van gegevens in elektronische vorm, die door een elektronisch apparaat onder één naam kan worden behandeld en aangesproken. Zoals een Word-bestand of MPEG-bestand. Zie ook de definitie van Bestand.
- Bedrijfsactiviteit: een taak die wordt uitgevoerd door een organisatie (Bron: NEN-ISO 30300:2020). Zie ook de specificatie van Bedrijfsactiviteit.
- Actor: Persoon, groep, organisatie of functionaris. Zie ook de specificatie van Actor.
- Locatie: Fysieke plaats in de ruimte. Zie ook de specificatie van Locatie.

In het onderstaande diagram zijn de in MDTO gespecificeerde relaties tussen de verschillende objecten weergegeven:

![test](/images/mdto_diagram_relaties.png)

### Aggregaties
Een informatieobject kan samengesteld zijn uit andere informatieobjecten. Dit wordt een aggregatie genoemd. Een archief omvat bijvoorbeeld alle informatieobjecten van één organisatie of persoon. Een dossier bevat alle informatieobjecten die op een bepaald onderwerp betrekking hebben. Een website bevat meerdere webpagina’s en een e-mail kan bijlagen bevatten. MDTO gaat ervan uit dat metagegevens bij elk aggregatieniveau zijn vastgelegd. Het is niet eenduidig wanneer een informatieobject als aggregatie beschouwd wordt. Bijvoorbeeld:

- Is een e-mail met een bijlage een ongedeeld informatieobject? Of is het een aggregatie met als onderdelen de tekst van de mail en de bijlage?
- Is een database met persoonsbeschrijvingen een ongedeeld informatieobject? Of is het een aggregatie met als onderdelen de beschrijvingen van alle individuele personen?
- Is een wet een ongedeeld informatieobject? Of is het een aggregatie met als onderdelen de artikelen in de wet?
- Is een verzameling van versies van een tekstdocument een ongedeeld informatieobject? Of is het een aggregatie met als onderdelen de losse versies?

Of een informatieobject wordt beschouwd als ongedeeld of als een aggregatie is een keuze waar MDTO geen regels voor geeft. Maar deze keuze heeft wel consequenties voor de metagegevens. Als een informatieobject als ondeelbaar wordt beschouwd, dan is het niet mogelijk om in MDTO-metagegevens onderscheid te maken tussen onderdelen van het informatieobject. Bijvoorbeeld als de versies van een tekstdocument geen afzonderlijke informatieobjecten zijn, dan hebben ze ook geen eigen creatiedatum. En als een wet of besluit ondeelbaar is, dan kunnen de artikelen geen eigen geldigheidsduur hebben. Als een mail ondeelbaar is, dan kunnen er voor de bijlage geen afzonderlijke beperkingen op de openbaarheid gelden.

### Overerving
MDTO kent geen overerving van metagegevens (attribuutwaarden) tussen aggregatieniveaus. Dit betekent dat bij de uitwisseling van MDTO-metagegevens attribuutwaarden op elk aggregatieniveau opgenomen moeten zijn. 

Wanneer overerving van metagegevens wordt toegepast is het door de tijd heen moeilijker te waarborgen dat individuele informatieobjecten alle gegevens bevatten. Dit wordt met name een probleem als de informatieobjecten buiten de grenzen van het systeem komen waarin zij zijn aangemaakt.

Omdat MDTO geen eisen stelt aan de manier waarop metagegevens worden vastgelegd, is het wel toegestaan om bij het vastleggen van de metagegevens overerving toe te passen. Mits zij bij de uitwisseling van deze metagegevens wel op elk aggregatieniveau worden genoemd. Een archiefvormer kan in een informatiesysteem bijvoorbeeld alleen op het hoogste aggregatieniveau worden vastgelegd. Bij een uitwisseling dient de archiefvormer dan wel op elk aggregatieniveau vermeld te worden.

### Bestanden
MDTO maakt onderscheid tussen een informatieobject als eenheid van informatie ongeacht de vorm, en de specifieke vorm waarin deze informatie wordt gerepresenteerd. Bestanden zijn één vorm van representatie (ook wel manifestatie genoemd). Maar een representatie kan bijvoorbeeld ook een papieren stuk of een videotape zijn. Andere vormen dan bestanden worden in MDTO verder niet behandeld.

De metagegevens die MDTO specificeert voor een informatieobject zijn onafhankelijk van haar representaties. Zoals de titel of auteur. De metagegevens die MDTO specificeert voor een bestand hebben specifiek betrekking op die representatie. Zoals het aantal bytes en het bestandsformaat. Door de metagegevens van informatieobject en representatie van elkaar te scheiden hoeven de representatieonafhankelijke metagegevens slechts één keer vastgelegd te worden. En kunnen in een later stadium gemakkelijk representaties toegevoegd worden aan een informatieobject.

Een informatieobject kan meerdere representaties hebben. Bijvoorbeeld een tekst kan gerepresenteerd worden door een Word-bestand én een PDF-bestand. Of een afbeelding door een bestand met hoge resolutie én een bestand met lage resolutie. De bestanden zijn verschillend, maar de informatie is dan hetzelfde. Om een informatieobject duurzaam toegankelijk te maken en houden, kan het nodig zijn om deze verschillende representaties te onderscheiden. Bijvoorbeeld omdat in de loop van de tijd een bestandsformaat niet meer ondersteund wordt. Of een PDF-bestand voor menselijke lezing en een XML-bestand voor machinale verwerking.

Het is ook mogelijk dat een informatieobject opgedeeld is in meerdere representaties. Bijvoorbeeld losse bestanden voor elke pagina van een gescand tekstdocument. Of een notitie als los bestand voor elke versie. Of een webpagina als een HTML-bestand en bestanden voor de afbeeldingen op de pagina. De representaties bevatten dan niet dezelfde inhoud.

Meestal is het zo dat representaties gekoppeld zijn aan een ongedeeld informatieobject. Maar ook aggregaties kunnen representaties hebben. Bijvoorbeeld een mailbox die beschouwd wordt als een aggregatie van mappen en daarbinnen mailberichten, kan als geheel gerepresenteerd worden door een Outlook-gegevensbestand (.pst-bestand). Of een website die beschouwd wordt als een aggregatie van webpagina’s, kan als geheel gerepresenteerd worden door een Web ARChive-bestand (WARC).

### Contextobjecten
MDTO specificeert alleen metagegevens voor informatieobjecten en bestanden. Maar onderscheidt daarbij wel verschillende soorten contextobjecten: bedrijfsactiviteit, actor en locatie. Omdat daar, vanuit de metagegevens van informatieobjecten, naar verwezen kan worden. Zoals naar de auteur van een tekstdocument of de locatie waar een informatieobject betrekking op heeft. Van deze contextobjecten worden, anders dan naam en identificatie, geen gegevens gespecificeerd in MDTO. 

## De structuur van metagegevens

### Attribuut-waardepaar
In MDTO is een enkel metagegeven bij een object gestructureerd als een attribuut-waardepaar. Bijvoorbeeld: 

* naam: ‘Rapport NL Digitaal - Data Agenda Overheid’ (bij een tekstdocument)
* omvang: 324534 (aantal bytes van een bestand)

Het attribuut in het paar is een eigenschap die een object kan hebben. Bijvoorbeeld “naam, ”omschrijving”, of “omvang”. In MDTO wordt een attribuut aangeduid met een tekenreeks zonder spaties.
 
De waarde in het paar is de waarde van het attribuut voor een specifiek object. Bijvoorbeeld “Jan de Boer” of “1802-06-17”. In MDTO kan de waarde van een attribuut bestaan uit:

* Een enkelvoudig gegeven.
* Een gegevensgroep (waaronder ook een begrip of een verwijzing).
  
In de attribuutspecificaties van MDTO wordt beschreven welke attribuut-waardeparen binnen MDTO voorkomen.


### Enkelvoudig gegeven
Een enkelvoudig gegeven is een gegeven dat binnen MDTO niet verder gestructureerd is. De enkelvoudig gegevens vormen de basis van de metagegevens. De enkelvoudige gegevens in  MDTO hebben de vorm van een XML built-in datatype (zie XML Schema Part 2: Datatypes). Bijvoorbeeld:

* ‘Jan de Boer’ (een string)
* 125000 (een integer)
* 2021-01-18 (een datum)

### Gegevensgroep
Een gegevensgroep is een samengesteld gegeven dat bestaat uit een opsomming  van attribuut-waardeparen. Een waarde kan zelf ook een gegevensgroep zijn, in dat geval is er sprake van nesting). Gegevensgroepen worden gebruikt als er meerdere enkelvoudige gegevens nodig zijn om de waarde van een attribuut weer te geven. Bijvoorbeeld:

**identificatie:** \
kenmerk: ‘9789047706205’ \
bron: ‘ISBN’ 
 
**checksum:** \
waarde:   ‘2C2D00B7ADC331709202290B7626D42759447800306307F452CE150E42CFB762’ \
algoritme: ‘SHA-256’ \
datum: ‘2011-04-13T21:11:18’

**betrokkene:**\
type relatie: ‘rechthebbende’ \
naam: ‘Architectenbureau Janssen’ 

**identificatie:**\
kenmerk: ‘99999988’ \
bron: ‘KVK’


### Verwijzing
Een verwijzing is een speciale gegevensgroep die gebruikt wordt om te verwijzen naar een ander object. Bijvoorbeeld een informatieobject die een verwijzing naar een representatie (een bestand) of naar een auteur (een actor) heeft. Een attribuut waarvan de waarde een verwijzing is wordt ook wel een relatie genoemd.

Een verwijzing heeft de volgende attributen:

* Naam: Een naam waarmee het object aangeduid wordt. Bedoeld voor menselijke lezing. Bijvoorbeeld “Jan de Boer” voor een actor, “Behandelen bouwvergunningen” voor een activiteit of “Binnenhof 1, 2513 AA Den Haag” voor een locatie. Omdat een naam niet uniek hoeft te zijn, kan het dubbelzinnig zijn welke object aangeduid wordt.
* Identiteit: Een of meerdere unieke identiteitskenmerken waarmee het object aangeduid wordt. Bedoeld voor menselijke of machinale lezing. Omdat de identificatie uniek is, wordt hiermee eenduidig het object aangeduid. Bij voorkeur is de identiteit zodanig dat op grond hiervan de metagegevens over het object gelokaliseerd kunnen worden. Maar MDTO stelt dat niet als eis.

Zie de specificatie van de gegevensgroepklasse verwijzingGegevens en de bijbehorende attributen voor de volledige beschrijving.

### Begrip
Een begrip is een speciale gegevensgroep die gebruikt wordt voor waarden waarvan de betekenis is vastgelegd in een zogenaamde begrippenlijst. Een begrip wordt gedefinieerd als een eenheid van denken (‘concept’ in [NEN-ISO 25964-1:2011)](https://www.nen.nl/nen-iso-25964-1-2011-en-163228). Begrippen hebben een betekenis en onderlinge semantische relaties die zijn vastgelegd in een begrippenlijst. Een begrip kan over elk concreet of abstract ding gaan waar we woorden aan geven en over communiceren. Begrippen worden in MDTO gebruikt als attribuutwaarde als het gewenst is de betekenis van die waarde vast te leggen. Zodat voor iedereen duidelijk is hoe die waarde geïnterpreteerd moet worden. Zoals de aanduidingen van informatietypes, categorieën in een classificatieschema of de categorieën in een selectielijst. Een begrippenlijst wordt ook wel een gecontroleerde woordenlijst genoemd.

Een begrip heeft de volgende attributen:

* label: De tekstweergave van het begrip dat is toegekend in de begrippenlijst.
* code: De code die aan het begrip is toegekend in de begrippenlijst.
* begrippenlijst: Verwijzing naar het informatieobject (de begrippenlijst) waarin de betekenis van het begrip is vastgelegd.
  
Zie de specificatie van de gegevensgroepklasse begripGegevens en de bijbehorende attributen voor de volledige beschrijving. 

### Klassespecificatie
Een klasse is een verzameling objecten (een objecttype), enkelvoudige gegevens (een datatype) of gegevensgroepen (een gegevensgroeptype). MDTO gebruikt klassen om vanuit de attribuutspecificaties te kunnen verwijzen naar een verzameling. Verder hebben klassen geen speciale betekenis binnen MDTO. 

Een klassespecificatie van objecten binnen MDTO bestaat uit de volgende onderdelen:

| Onderdelen   | Beschrijving                                                                                                                                                                                   |
| ------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Naam         | De naam van de klasse. Deze wordt gebruikt om naar de klasse te verwijzen. De naam is een tekenreeks zonder spaties. Voor objectklassen wordt de naamgevingsconventie UpperCamelCase gebruikt. |
| Definitie    | Beschrijving van de betekenis van de klasse.                                                                                                                                                   |
| Regels       | Nadere eisen waaraan moet worden voldaan.                                                                                                                                                      |
| Overerft van | Vermelding van de bovenliggende klasse waarvan de attributen worden overerft. (Merk op dat MDTO geen overerving van attribuutwaarden van bovenliggende aggregatieniveaus kent.).               |
| Attributen   | Opsomming van de attributen die in MDTO voor deze klasse zijn gespecificeerd.                                                                                                                  |
| Toelichting  | Nadere toelichting op de definitie. De toelichting is alleen bedoeld ter verduidelijking en bevat geen extra eisen aan het object.                                                             |
| Voorbeelden  | Voorbeelden van elementen van de klasse.                                                                                                                                                       |

### Attribuutspecificatie
Een attribuutspecificatie beschrijft de betekenis en de toegestane waarden van een attribuut dat in MDTO-metagegevens voor kan komen. 

Een attribuutspecificatie bestaat uit de volgende onderdelen:

| Onderdelen     | Beschrijving                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| -------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Naam           | De naam van het attribuut. Deze wordt gebruikt om naar het attribuut te verwijzen. De naam is een tekenreeks zonder spaties. Voor attributen wordt de naamgevingsconventie lowerCamelCase gebruikt.                                                                                                                                                                                                                                                                                                                                          |
| Label          | De naam van het attribuut voor menselijke lezing.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| Domein         | De klasse van objecten of gegevensgroepen waar dit attribuut een waarde voor kan hebben.                                                                                                                                                                                                                                                                                                                                                                                                                                                     | De klasse van objecten of gegevensgroepen waar dit attribuut een waarde voor kan hebben.                                                                                                                                                                                                                                                                                               |
| Bereik         | De klasse(n) van waarden die toegestaan zijn voor het attribuut. Dit kan een datatype of een gegevensgroepklasse zijn. In een aantal gevallen zijn meerdere datatypen toegestaan.                   Als het bereik “Verwijzing” is, dan is daarbij ook aangegeven naar welke klasse objecten verwezen wordt door dit attribuut. Bijvoorbeeld “Verwijzing (Bestand)” is een verwijzing naar een bestand”.                                                                                                                                     | De klasse(n) van waarden die toegestaan zijn voor het attribuut. Dit kan een datatype of een gegevensgroepklasse zijn. In een aantal gevallen zijn meerdere datatypen toegestaan. Als het bereik “Verwijzing” is, dan is daarbij ook aangegeven naar welke klasse objecten verwezen wordt door dit attribuut. Bijvoorbeeld “Verwijzing (Bestand)” is een verwijzing naar een bestand”. |
| Doel           | Waarom het van belang is om dit attribuut op te nemen in metagegevens. Vanuit het perspectief van duurzame toegankelijkheid. Bij de attributen van een gegevensgroep wordt geen doel vermeld.                                                                                                                                                                                                                                                                                                                                                |
| Definitie      | De betekenis van het attribuut.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| Begrippenlijst | Als het bereik “begripGegevens” is, dan is hier aangegeven welke begrippenlijsten zijn toegestaan voor dit attribuut. Mogelijk zijn: <ul><li>“Gesloten: ” + begrippenlijst: Alleen de aangegeven begrippenlijst mag gebruikt worden. Uitbreiding hiervan is niet toegestaan. <li>“Open: ” + begrippenlijst: De aangegeven begrippenlijst mag gebruikt worden of een uitbreiding hiervan. Een uitbreiding wil zeggen dat er extra begrippen met een andere betekenis zijn toegevoegd aan de aangegeven begrippenlijst.  </ul>                 |
| Verplichting   | Of het attribuut een waarde moet hebben. Mogelijk zijn: <ul><li>“Verplicht”: Het attribuut moet altijd een waarde hebben.  <li>“Verplicht, indien bekend”: Het attribuut moet een waarde hebben, als deze binnen de verantwoordelijke organisatie noodzakelijk is voor het uitvoeren van werkprocessen en taken, bekend is of afgeleid kan worden van andere bekende gegevens. Tenzij hier redelijkerwijs niet aan voldaan kan worden. Zie voor een toelichting op “verplicht, indien bekend” het onderdeel Definitie van MDTO-conform.</ul> |
| Herhaalbaar    | Of het attribuut voor een object meerdere waarden mag hebben. Mogelijke waarden “ja” of “nee”.                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| Regels         | Nadere eisen waar de waarden van dit attribuut aan moeten voldoen. Hierin kan verwezen worden naar waarden van andere attributen.                                                                                                                                                                                                                                                                                                                                                                                                            |
| Toelichting    | Waar nodig, een toelichting ter verduidelijking van de specificatie. Een toelichting is alleen ter verduidelijking en bevat geen extra eisen.                                                                                                                                                                                                                                                                                                                                                                                                |
| Voorbeelden    | Voorbeelden van mogelijke waarden. De voorbeelden zijn alleen ter verduidelijking en bevatten geen extra eisen. Als het bereik een gegevensgroepklasse is, dan bevat de specificatie meestal geen voorbeelden. Die zijn dan opgenomen bij de attributen van de gegevensgroep.                                                                                                                                                                                                                                                                |                                                                                                                                                                                                                                                                                                                                                                                        |

### Datatypen
De volgende datatypen worden gebruikt in de attribuutspecificaties van MDTO.

Alle  datatypen zijn ingebouwde (built-in) datatypen gedefinieerd in XML Schema.

| naam       | toelichting                                                                                                                                                                                                                                                                                                     |
| ---------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| date       | datum uitgedrukt als yyyy-mm-dd conform iso 8601. voorbeeld: 1976-06-13 (13 juni 1976)                                                                                                                                                                                                                          |
| gYear      | periode van één kalenderjaar conform iso 8601. voorbeeld: 1993                                                                                                                                                                                                                                                  |
| gYearMonth | periode van één kalendermaand in een specifiek jaar conform iso 8601. voorbeeld: 2001-11 (november 2001)                                                                                                                                                                                                        |
| dateTime   | datum- en tijd uitgedrukt in yyyy-mm-ddThh:mm:ss conform iso 8601. voorbeeld: 2014-07-24T08:03:01 (24 juli 2014 8 uur, 3 minuten en 1 seconde)                                                                                                                                                                  |
| duration   | periode in tijd uitgedrukt conform iso 8601. voorbeeld: P70Y (70 jaar), of P0Y0M14D (14 dagen)                                                                                                                                                                                                                  |
| anyURI     | uri conform rfc 3987. uri staat voor unique resource identifier. het is een gestandaardiseerde manier om te verwijzen naar een stuk data (zoals webpagina’s met informatie, objecten en datasets) en hier direct toegang toe te geven. een url is een voorbeeld van een uri. voorbeeld: https://www.example.com |
| language   | identificatiekenmerk van een natuurlijke taal conform rfc 3066. voorbeeld: nl (nederland)                                                                                                                                                                                                                       |
| string     | een reeks tekens of karakters. een lege string wordt opgevat als een ontbrekende waarde. in mdto zijn lege strings daarom niet toegestaan. voorbeeld: “abc 123”                                                                                                                                                 |
| integer    | geheel getal, lengte is minimaal 1 en maximale lengte is onbepaald, zonder voorloopnullen. subtype van iso number (iso 11404). voorbeeld: 23042                                                                                                                                                                 |