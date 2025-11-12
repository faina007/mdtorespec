Een op zichzelf staand geheel van gegevens met een eigen identiteit.

- Overerft van Object

**Attributen**
| Attribuut                      | Omschrijving                                                                          | Verplicht | Herhaalbaar | Datatype                      |
| ------------------------------ | ------------------------------------------------------------------------------------- | --------- | ----------- | ----------------------------- |
| `aggregatieniveau`             | Het niveau van samenstelling van het informatieobject.                                | Nee       | Nee         | `xsd:string`                  |
| `classificatie`                | De toegepaste classificatie of categorie van het informatieobject.                    | Nee       | Ja          | `xsd:string`                  |
| `trefwoord`                    | Kernwoord of onderwerp waarmee het informatieobject wordt beschreven.                 | Nee       | Ja          | `xsd:string`                  |
| `omschrijving`                 | Beschrijving van de inhoud of betekenis van het informatieobject.                     | Nee       | Nee         | `xsd:string`                  |
| `raadpleeglocatie`             | Verwijzing naar de locatie waar het informatieobject geraadpleegd kan worden.         | Nee       | Nee         | `raadpleeglocatieGegevens`    |
| `dekking in tijd`              | De periode waarop het informatieobject betrekking heeft.                              | Nee       | Nee         | `tijdGegevens`                |
| `dekking in ruimte`            | De geografische reikwijdte van het informatieobject.                                  | Nee       | Nee         | `ruimteGegevens`              |
| `taal`                         | De gebruikte taal of talen binnen het informatieobject.                               | Nee       | Ja          | `xsd:language`                |
| `event`                        | Gebeurtenis waarmee het informatieobject in verband staat.                            | Nee       | Ja          | `eventGegevens`               |
| `waardering`                   | De waardering of beoordeling van het informatieobject.                                | Nee       | Nee         | `waarderingGegevens`          |
| `bewaartermijn`                | De termijn waarvoor het informatieobject bewaard dient te blijven.                    | Nee       | Nee         | `xsd:duration`                |
| `informatiecategorie`          | De categorie of soort informatieobject.                                               | Nee       | Nee         | `xsd:string`                  |
| `is onderdeel van`             | Verwijzing naar het overkoepelende informatieobject waarvan dit object deel uitmaakt. | Nee       | Nee         | `verwijzingGegevens`          |
| `bevat onderdeel`              | Verwijzing naar onderliggende informatieobjecten.                                     | Nee       | Ja          | `verwijzingGegevens`          |
| `heeft representatie`          | Verwijzing naar de fysieke of digitale representaties van het informatieobject.       | Nee       | Ja          | `verwijzingGegevens`          |
| `gerelateerd informatieobject` | Verwijzing naar andere relevante informatieobjecten.                                  | Nee       | Ja          | `verwijzingGegevens`          |
| `aanvullende metagegevens`     | Extra metadata die niet in andere attributen passen.                                  | Nee       | Ja          | `aanvullendeMetagegevensType` |
| `archiefvormer`                | De organisatie of persoon die het informatieobject heeft gevormd.                     | Nee       | Ja          | `verwijzingGegevens`          |
| `betrokkene`                   | De persoon of organisatie die verband houdt met het informatieobject.                 | Nee       | Ja          | `verwijzingGegevens`          |
| `activiteit`                   | De handeling of taak waaruit het informatieobject is voortgekomen.                    | Nee       | Ja          | `verwijzingGegevens`          |
| `beperking gebruik`            | Eventuele beperkingen op het gebruik of de toegang van het informatieobject.          | Nee       | Ja          | `beperkingGebruikType`        |

**Toelichting**

- Informatieobjecten binnen de context van **MDTO** zijn gegevensobjecten die ontstaan uit de uitvoering van **overheidstaken**.  
De term *informatieobject* komt in wet- en regelgeving ook voor als **archiefstuk** of **document**.  
- Een informatieobject dat bestaat uit meerdere kleinere informatieobjecten wordt beschouwd als een **aggregatie**.

**Voorbeelden**

- Een document  
- Een database  
- Een dossier  
- Een website  