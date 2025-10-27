# 📘 MDTO – Metadata voor Duurzaam Toegankelijke Overheidsinformatie

Het **MDTO (Metadata voor Duurzaam Toegankelijke Overheidsinformatie)** is een XML-schema ontwikkeld door het [Nationaal Archief](https://www.nationaalarchief.nl/archiveren/mdto) om de duurzame toegankelijkheid van digitale overheidsinformatie te ondersteunen.  
Het schema beschrijft de structuur en betekenis van metadata die nodig zijn om informatieobjecten op een gestandaardiseerde manier te registreren, beheren en raadplegen.

---

## 🧩 Doel van het schema

Het MDTO-schema heeft als doel om:
- de **uitwisselbaarheid** van metadata tussen organisaties te verbeteren;  
- de **duurzame toegankelijkheid** van digitale informatieobjecten te waarborgen;  
- een **eenduidige structuur** te bieden voor de registratie van informatieobjecten, bestanden en gerelateerde gegevens.

---

## 📄 Inhoud van deze repository

| Bestand / map | Beschrijving |
|----------------|--------------|
| `/schema/` | Bevat de XSD-bestanden van de huidige versie van het MDTO-schema. |
| `/examples/` | Voorbeelden van XML-bestanden die voldoen aan het MDTO-schema. |
| `README.md` | Deze documentatie. |
| `CHANGELOG.md` | Overzicht van wijzigingen per schema-versie. |

---

## 🏷️ Versiebeheer

De changelog met alle wijzigingen tussen schema-versies wordt bijgehouden in [`CHANGELOG.md`](./CHANGELOG.md).  
De inline changelog die eerder in het XML-schema stond, is verwijderd en wordt voortaan beheerd via deze GitHub-omgeving.

---

## ⚙️ Gebruik

1. **Valideer XML-bestanden** tegen het schema:  
   ```bash
   xmllint --noout --schema mdto.xsd voorbeeld.xml
