# Ausdruckprotokoll

Im Tab **„Ausdruckprotokoll"** wird der PDF-Bericht für die Schutzraumbemessung erzeugt.

![Screenshot: Tab Ausdruckprotokoll](screenshots/07_ausdruckprotokoll.png)

---

## Protokollumfang und Darstellung

| Option | Beschreibung |
|---|---|
| **Vollständiges Ausdruckprotokoll** | Vollversion mit allen Berichtsteilen |
| **Kurzfassung** | Kompakte Version mit reduziertem Umfang |

### Darstellungsart Schnittgrössen (nur Vollversion)

| Option | Beschreibung |
|---|---|
| **Isoflächen** | Flächenhafte Farbdarstellung (Standard) |
| **Isolinien** | Darstellung mit Konturlinien |

> **Hinweis:** Bei **Kurzfassung** wird die Auswahl **Darstellungsart Schnittgrössen** ausgeblendet.

---

## Kontaktdaten (linke Seite)

Die Kontaktdaten werden für vier Rollen erfasst:

| Rolle | Felder |
|---|---|
| **Bauherr** | Name, Strasse, PLZ/Ort, E-Mail, Telefon |
| **Architekt** | Name, Strasse, PLZ/Ort, E-Mail, Telefon |
| **Ingenieur** | Name, Strasse, PLZ/Ort, E-Mail, Telefon |
| **Prüfingenieur** | Name, Strasse, PLZ/Ort, E-Mail, Telefon |

Pflichtfelder für die PDF-Erzeugung sind je Rolle:

- **Name**
- **Strasse**
- **PLZ/Ort**

E-Mail und Telefon sind optional.

Die Kontaktdaten werden automatisch gespeichert und beim nächsten Öffnen wieder geladen.

---

## PDF erzeugen

1. Protokollumfang (und ggf. Darstellungsart) wählen.
2. Pflichtfelder in den Kontaktdaten ausfüllen.
3. Auf **„Ausdruckprotokoll erzeugen"** klicken (oder den Status-Kreis).
4. **Speicherort wählen** – ein Dateidialog öffnet sich.
   - Vorgeschlagener Dateiname: `{Projektname} TWKDok.pdf`
   - Bei Englisch wird `_en` ergänzt.
   - Bei Kurzfassung wird `Kurzversion` ergänzt.
5. Die Erzeugung läuft; ein Fortschrittsdialog zeigt den Stand.
6. Nach Abschluss erscheint eine Erfolgsmeldung mit dem Speicherpfad.

### Status-Anzeige

| Symbol | Bedeutung |
|---|---|
| 🔵 Blauer Kreis | Bereit – PDF kann erzeugt werden |
| 🟢 Grüner Kreis (✓) | PDF erfolgreich erzeugt |
| 🔴 Roter Kreis (✗) | Fehler beim Erzeugen (erneuter Versuch möglich) |

---

## Inhalt des PDF-Berichts

### Deckblatt
- Projektname, 3D-Ansicht, Kontaktdaten, Datum

### Kapitel 1: Grundlagen
- Normen (TWK 2017, SIA 262, SIA 261)
- Bemessungsart, Software-Versionen
- Baustoffe (Beton und Stahl)
- Baugrund und Grundwasser
- Gebäudedaten und Bauteile-Übersicht
- 3D-Ansicht und Bewehrungszusammenfassung

### Kapitel 2: Lastfälle und Lastkombinationen (nur Vollversion)
- Screenshots der Lastfälle aus AxisVM
- Tabellen der Lastkombinationen mit Faktoren

### Kapitel 3+: Bauteile (je ein Kapitel pro Bauteil)
- Allgemeine Parameter des Bauteils
- Schichtaufbau und äquivalente Dicke
- Bewehrungsparameter
- Biegebemessung: Skizzen, Momentendiagramme, Ausnutzung, Nachweistabellen
- Schubbemessung: Skizzen, Schubkraftdiagramme, Ausnutzung, Nachweistabellen

![Screenshot: PDF-Beispiel](screenshots/07_pdf_beispiel.png)

