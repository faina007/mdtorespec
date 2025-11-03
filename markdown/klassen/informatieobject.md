> Een op zichzelf staand geheel van gegevens met een eigen identiteit.

- Overerft van Object

**Attributen**
| Attribuut                      | Omschrijving                                                                          | Verplicht                | Herhaalbaar              | Datatype                      |
| ------------------------------ | ------------------------------------------------------------------------------------- | ------------------------ | ------------------------ | ----------------------------- |
| `aggregatieniveau`             | Het niveau van samenstelling van het informatieobject.                                | :heavy_multiplication_x: | :heavy_multiplication_x: | `xsd:string`                  |
| `classificatie`                | De toegepaste classificatie of categorie van het informatieobject.                    | :heavy_multiplication_x: | :heavy_check_mark:       | `xsd:string`                  |
| `trefwoord`                    | Kernwoord of onderwerp waarmee het informatieobject wordt beschreven.                 | :heavy_multiplication_x: | :heavy_check_mark:       | `xsd:string`                  |
| `omschrijving`                 | Beschrijving van de inhoud of betekenis van het informatieobject.                     | :heavy_multiplication_x: | :heavy_multiplication_x: | `xsd:string`                  |
| `raadpleeglocatie`             | Verwijzing naar de locatie waar het informatieobject geraadpleegd kan worden.         | :heavy_multiplication_x: | :heavy_multiplication_x: | `raadpleeglocatieGegevens`    |
| `dekking in tijd`              | De periode waarop het informatieobject betrekking heeft.                              | :heavy_multiplication_x: | :heavy_multiplication_x: | `tijdGegevens`                |
| `dekking in ruimte`            | De geografische reikwijdte van het informatieobject.                                  | :heavy_multiplication_x: | :heavy_multiplication_x: | `ruimteGegevens`              |
| `taal`                         | De gebruikte taal of talen binnen het informatieobject.                               | :heavy_multiplication_x: | :heavy_check_mark:       | `xsd:language`                |
| `event`                        | Gebeurtenis waarmee het informatieobject in verband staat.                            | :heavy_multiplication_x: | :heavy_check_mark:       | `eventGegevens`               |
| `waardering`                   | De waardering of beoordeling van het informatieobject.                                | :heavy_multiplication_x: | :heavy_multiplication_x: | `waarderingGegevens`          |
| `bewaartermijn`                | De termijn waarvoor het informatieobject bewaard dient te blijven.                    | :heavy_multiplication_x: | :heavy_multiplication_x: | `xsd:duration`                |
| `informatiecategorie`          | De categorie of soort informatieobject.                                               | :heavy_multiplication_x: | :heavy_multiplication_x: | `xsd:string`                  |
| `is onderdeel van`             | Verwijzing naar het overkoepelende informatieobject waarvan dit object deel uitmaakt. | :heavy_multiplication_x: | :heavy_multiplication_x: | `verwijzingGegevens`          |
| `bevat onderdeel`              | Verwijzing naar onderliggende informatieobjecten.                                     | :heavy_multiplication_x: | :heavy_check_mark:       | `verwijzingGegevens`          |
| `heeft representatie`          | Verwijzing naar de fysieke of digitale representaties van het informatieobject.       | :heavy_multiplication_x: | :heavy_check_mark:       | `verwijzingGegevens`          |
| `gerelateerd informatieobject` | Verwijzing naar andere relevante informatieobjecten.                                  | :heavy_multiplication_x: | :heavy_check_mark:       | `verwijzingGegevens`          |
| `aanvullende metagegevens`     | Extra metadata die niet in andere attributen passen.                                  | :heavy_multiplication_x: | :heavy_check_mark:       | `aanvullendeMetagegevensType` |
| `archiefvormer`                | De organisatie of persoon die het informatieobject heeft gevormd.                     | :heavy_multiplication_x: | :heavy_check_mark:       | `verwijzingGegevens`          |
| `betrokkene`                   | De persoon of organisatie die verband houdt met het informatieobject.                 | :heavy_multiplication_x: | :heavy_check_mark:       | `verwijzingGegevens`          |
| `activiteit`                   | De handeling of taak waaruit het informatieobject is voortgekomen.                    | :heavy_multiplication_x: | :heavy_check_mark:       | `verwijzingGegevens`          |
| `beperking gebruik`            | Eventuele beperkingen op het gebruik of de toegang van het informatieobject.          | :heavy_multiplication_x: | :heavy_check_mark:       | `beperkingGebruikType`        |


**Toelichting**

- Informatieobjecten binnen de context van **MDTO** zijn gegevensobjecten die ontstaan uit de uitvoering van **overheidstaken**.  
De term *informatieobject* komt in wet- en regelgeving ook voor als **archiefstuk** of **document**.  

- Een informatieobject dat bestaat uit meerdere kleinere informatieobjecten wordt beschouwd als een **aggregatie**.

**Voorbeelden**

- Een document  
- Een database  
- Een dossier  
- Een website  