# DRAMERA v4.17 - Changelog (Testphase 2)

**Datum:** 27. Januar 2026  
**Vorherige Version:** DramaNet Werkbank v4.16

---

## UMBENENNUNG

- **DramaNet → Dramera** (Namensänderung wegen Markenschutz)
- Alle Vorkommen von "DramaNet" durch "Dramera" ersetzt
- Neues Logo: Gestapelt DRA/MERA in Georgia-Schrift
  - Akzentfarbe: #C4956A (warm-gold)
  - Textfarbe: #4A4035 (dunkelbraun)

---

## LOGO-INTEGRATION

### Positionen:
1. **Header** - zentral, 44px, `position: absolute`
2. **Schreibfläche** - links oben, 38px, 70% Opazität
3. **Ladebildschirm** - gross, animiert (pulse)
4. **Favicon** - SVG mit hellem Hintergrund

### Logo-Dateien:
- `dramera-logo.svg` - Standard (transparenter Hintergrund)
- `dramera-logo-dark.svg` - Für dunkle Hintergründe
- `dramera-logo-with-bg.svg` - Mit hellem Hintergrund

---

## WIKI & GLOSSAR FIXES

### Offene Form Werkzeuge:
- **Problem:** Wiki-Buttons öffneten Wiki ohne konkreten Artikel
- **Lösung:** Einträge in GLOSSARY hinzugefügt (verweisen auf ausführliche WIKI_ENTRIES)
- Betroffen: Sprechinstanzen, Textflächen, Materialcollage, Spracharbeit, Performativität

### Emotionale Bewegung:
- Wiki-Link korrigiert: `transformation` → `emotionale_bewegung`

### Intrige:
- Doppelten GLOSSARY-Eintrag entfernt (Zeile 3297)
- Ausführlicher Artikel nach Peter von Matt bleibt bestehen

---

## TEXTE ÜBERARBEITET

### Schreibflächen-Hilfetext (sachlich, ohne "Du"):
```
📝 Willkommen bei Dramera!

Wer schon weiss, was erzählt werden soll – hier direkt losschreiben.

Noch auf der Suche? Oben zu «Geführt» wechseln.

LINKS: Material direkt eingeben (Vorgaben, Figuren, Themen, Szenen-Ideen).

RECHTS: Werkzeuge vertiefen einzelne Aspekte (Konflikt, Prämisse, Struktur...).

TIPP: Text markieren → mit +Figur / +Thema / +Szene ins Material übernehmen.

FERTIG GESAMMELT? Zu «Ordnen» wechseln und den Zeitstrahl bauen.

📚 Wiki: Erklärungen zu allen Begriffen.
❓ Fragezeichen: Ausführliche Anleitung.
🤖 KI-Funktionen: Einstellungen → API-Key.
```

### Anleitung im Wiki:
- Komplett sachlich umformuliert (kein "Du")
- Neue Sektion: "So erhält man einen Anthropic API-Key" (Schritt-für-Schritt)

---

## DATEIEN

| Datei | Beschreibung |
|-------|--------------|
| `dramera-werkbank-v4_17.jsx` | React-Komponente (31.307 Zeilen) |
| `dramera-v4_17.html` | Standalone HTML mit eingebettetem React |
| `dramera-logo.svg` | Logo Standard |
| `dramera-logo-dark.svg` | Logo für Dark Mode |
| `dramera-logo-with-bg.svg` | Logo mit Hintergrund |

---

## TECHNISCHE DETAILS

- **Zeilen:** 31.307
- **Dateigrösse JSX:** ~1.4 MB
- **Dateigrösse HTML:** ~1.4 MB
- **React Version:** 18
- **Babel:** Standalone (Browser-Kompilierung)

---

## BEKANNTE ISSUES / TODO (Testphase 3)

- [ ] Schauplatz & Zeit: Infoboxen in den Feldern
- [ ] Konflikt: Infoboxen in den Feldern
- [ ] Themenstern: Grafische Darstellung wie WiseMapping
- [ ] Mobile Optimierung prüfen

---

## KONTEXT FÜR NÄCHSTE SESSION

Diese Datei dient als Referenz für zukünftige Chat-Sessions. 

**Wichtige Dateipfade:**
- Hauptdatei: `/home/claude/dramera-werkbank-v4_17.jsx`
- GLOSSARY: ab Zeile ~3200
- WIKI_ENTRIES: ab Zeile ~3300
- Offene Form Tools: ab Zeile ~19700
- Header/Logo: ab Zeile ~27880
- Schreibfläche: ab Zeile ~28035
- CSS Styles: ab Zeile ~20280

**Wichtige Konzepte:**
- GLOSSARY = kurze Einträge (für Suche/Liste)
- WIKI_ENTRIES = ausführliche Artikel (merged mit GLOSSARY)
- Kein doppelter Key erlaubt (JS-Objekt - späterer überschreibt)
