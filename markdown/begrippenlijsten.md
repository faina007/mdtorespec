# Begrippenlijsten

## Aggregatieniveaus
Type begrippenlijst: Open \
Deze begrippenlijst wordt gebruikt binnen het attribuut aggregatieniveau

| Label       | Definitie                                                                                                                                                                                                                                        |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Archief     | Geheel van informatieobjecten, ontvangen of opgemaakt door een archiefvormer.                                                                                                                                                                    |
| Serie       | Verzameling van dossiers, fysieke archiefbestanddelen en/of stukken, numeriek, alfabetisch, chronologische of logisch geordend, ontstaan vanuit een identieke "handeling", dan wel een identieke vorm hebbend dan wel verwante inhoud bevattend. |
| Dossier     | Geheel van fysieke of virtueel gekoppelde informatieobjecten die op één onderwerp betrekking hebben.                                                                                                                                             |
| Archiefstuk | Enkelvoudig informatieobject of informatie-eenheid. Enkelvoudig wil zeggen dat het stuk niet meer dan één component bevat.                                                                                                                       |


## EventTypeLijst
Type begrippenlijst: Open \
Deze begrippenlijst wordt gebruikt binnen het attribuut eventType

| Label                  | Definitie                                                                                                                                                                                                                              |
| ---------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Creatie                | Creatie van een informatieobject door een auteur.                                                                                                                                                                                      |
| Ontvangst              | Ontvangst van een informatieobject door de archiefvormer.                                                                                                                                                                              |
| Verzending             | Verzending van een informatieobject door de archiefvormer.                                                                                                                                                                             |
| Opname                 | Opname van een informatieobject in een applicatie met de bijbehorende metagegevens. De opname vindt bijvoorbeeld plaats na creatie of ontvangst en wordt gerealiseerd door registratie en opslaan.                                     |
| Digitalisering         | Het scannen van een fysiek informatieobject, waardoor een digitaal informatieobject ontstaat.                                                                                                                                          |
| Vervanging             | Formele vervanging van een informatieobject door een ander informatieobject, waarbij het vervangende informatieobject de plaats en archiefwettelijke status overneemt en het originele informatieobject die plaats en status verliest. |
| Bevriezing             | ‘Bevriezen’ van het informatieobject, waarna geen wijzigingen meer zijn toegestaan. Voorbeelden zijn afsluiten van dossier of afronden van een tekstdocument.                                                                          |
| Conversie              | Omzetting van het informatieobject van het ene naar het andere formaat.                                                                                                                                                                |
| Export                 | Exporteren van een informatieobject en de metagegevens uit de applicatie.                                                                                                                                                              |
| Import                 | Importeren van een informatieobject met de metagegevens uit de applicatie.                                                                                                                                                             |
| Kopie                  | Kopiëren van een informatieobject met de metagegevens binnen de applicatie zodat een nieuw informatieobject ontstaat. NB: unieke metagegevens worden bij een kopie wel gewijzigd.                                                      |
| Migratie               | Verplaatsen van het informatieobject van de ene hard- en/of softwareconfiguratie naar een andere, zonder het formaat te wijzigen.                                                                                                      |
| Vernietigen            | Vernietigen van informatie is het blijvend ontoegankelijk maken van die informatie, waardoor deze niet meer vindbaar, beschikbaar, leesbaar, interpreteerbaar en betrouwbaar is.                                                       |
| Overbrenging           | Formeel overbrengen van het informatieobject en bijbehorende metagegevens naar een archiefbewaarplaats, waarbij het zorgdragerschap ook wordt overgedragen.                                                                            |
| Uitplaatsing           | Uitplaatsen van een informatieobject en bijbehorende metagegevens naar een beheeromgeving buiten de eigen organisatie, zonder daarbij het zorgdragerschap over te dragen.                                                              |
| Wijziging              | Wijzigen van het informatieobject of de bijbehorende metagegevens.                                                                                                                                                                     |
| Publicatie             | Publiceren van het informatieobject en bijbehorende metagegevens, bijvoorbeeld op een openbare webpagina.                                                                                                                              |
| Accordering            | Het accorderen van een informatieobject. Dit kan bijvoorbeeld door een digitale handtekening.                                                                                                                                          |
| Validatie Handtekening | Controle of de digitale handtekening daadwerkelijk door de desbetreffende actor is gezet.                                                                                                                                              |

## Waarderingen
Type begrippenlijst: Gesloten \
Deze begrippenlijst wordt gebruikt binnen het attribuut waardering.

| Code | Label                | Definitie                                                                                                                         |
| ---- | -------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| B    | Blijvend te bewaren  | Het informatieobject dient blijvend bewaard te worden.                                                                            |
| V    | Tijdelijk te bewaren | Het informatieobject dient tijdelijk bewaard te worden en na afloop van de bewaartermijn vernietigd te worden.                    |
| N    | Nader te bepalen     | Er is mogelijk een waardering, maar de aard daarvan is niet vastgelegd als type waardering en niet vastgelegd in de metagegevens. |

## Relatietypen (betrokkene)
Type begrippenlijst: Open \ 
Deze begrippenlijst wordt gebruikt binnen het attribuut betrokkeneTypeRelatie.

| Label          | Definitie                                                                                                                                                                                                                                                                             |
| -------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Belanghebbende | De persoon of organisatie die een belang heeft bij de inhoud van het informatieobject. Bijvoorbeeld als iemand het onderwerp is van een informatieobject, of wanneer het informatieobject een besluit betreft dat het belang van een persoon of organisatie direct of indirect treft. |
| Indiener       | Indiener van een verzoek of aanvraag waar het informatieobject betrekking op heeft.                                                                                                                                                                                                   |
| Rechthebbende  | Degene die een wettelijk recht op het informatieobject kan laten gelden, zoals auteurs- of portretrecht.                                                                                                                                                                              |


## Relatietypen (informatieobject)
Type begrippenlijst: Open \
Deze begrippenlijst wordt gebruikt binnen het attribuut gerelateerdInformatieobjectTypeRelatie.

| Label                 | Betekenis                                                                                                                                     | Overeenkomstig Dublin Core label |
| --------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------- |
| Heeft Versie          | Een gerelateerd object dat een versie, editie of een aanpassing is van het beschreven object.                                                 | `dcterms:hasVersion`             |
| Wordt aangehaald door | Een gerelateerd object dat refereert aan, citeert of op een andere wijze verwijst naar het beschreven object.                                 | `dcterms:isReferencedBy`         |
| Is vervangen door     | Een gerelateerd object dat het beschreven object vervangt, verdringt of opvolgt.                                                              | `dcterms:isReplacedBy`           |
| Is vereist door       | Een gerelateerd object dat het beschreven object nodig heeft ter ondersteuning van de functie, levering of coherentie.                        | `dcterms:isRequiredBy`           |
| Is een versie van     | Een gerelateerd object waarvan het beschreven object een versie, editie of een aanpassing is.                                                 | `dcterms:isVersionOf`            |
| Refereert aan         | Een gerelateerd object waarnaar wordt gerefereerd, uit wordt geciteerd of op een andere wijze naar wordt verwezen door het beschreven object. | `dcterms:references`             |
| Vervangt              | Een gerelateerd object dat wordt vervangen, verdrongen of opgevolgd door het beschreven object.                                               | `dcterms:replaces`               |
| Heeft nodig           | Een gerelateerd object dat het beschreven object nodig heeft ter ondersteuning van de functie, levering of coherentie.                        | `dcterms:requires`               |

## BeperkingGebruikTypeLijst
Type begrippenlijst: Open \
Deze begrippenlijst wordt gebruikt binnen het attribuut beperkingGebruikType. 

| Label            | Definitie                                                                                                                                                                  |
| ---------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Geen beperking   | Er rust geen beperking op het gebruik van het informatieobject.                                                                                                            |
| Nader te bepalen | Er is mogelijk een beperking, maar de aard daarvan is niet vastgelegd als type beperking en niet vastgelegd in de metagegevens.                                            |
| Overig           | Niet nader gespecificeerde beperking. Deze waarde wordt gebruikt als er geen ander geschikt type gedefinieerd is en er in de documentatie wel een beperking is omschreven. |

## ChecksumAlgoritme
Type begrippenlijst: Open \
Deze begrippenlijst wordt gebruikt binnen het attribuut checksumAlgoritme.

| Label   | Definitie                                                                                                                                                                            |
| ------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| SHA-224 | Cryptografisch hashalgoritme ten behoeve van authenticatie en integriteitscontrole. Zie [Forum Standaardisatie – SHA-2](https://www.forumstandaardisatie.nl/open-standaarden/sha-2). |
| SHA-256 | Cryptografisch hashalgoritme ten behoeve van authenticatie en integriteitscontrole. Zie [Forum Standaardisatie – SHA-2](https://www.forumstandaardisatie.nl/open-standaarden/sha-2). |
| SHA-384 | Cryptografisch hashalgoritme ten behoeve van authenticatie en integriteitscontrole. Zie [Forum Standaardisatie – SHA-2](https://www.forumstandaardisatie.nl/open-standaarden/sha-2). |
| SHA-512 | Cryptografisch hashalgoritme ten behoeve van authenticatie en integriteitscontrole. Zie [Forum Standaardisatie – SHA-2](https://www.forumstandaardisatie.nl/open-standaarden/sha-2). |
