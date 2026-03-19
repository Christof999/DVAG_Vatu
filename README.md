# DVAG Kontaktformular - Vatu

Ein professionelles Kontaktformular im Corporate Design der Deutschen Vermögensberatung AG (DVAG) mit Firebase-Integration zur automatischen Speicherung von Kundenanfragen.

## 🎯 Features

- ✅ **Professionelles DVAG-Design** mit Gold, Grau und Weiß
- ✅ **Vollständiges Kontaktformular** mit Name, Telefon, E-Mail und Nachricht
- ✅ **Portrait-Sektion** für Vaathulan Perinparajah mit Beschreibung
- ✅ **Firebase-Integration** zur automatischen Datenspeicherung
- ✅ **E-Mail-Benachrichtigungen** via EmailJS an christof.didi@googlemail.com
- ✅ **Echtzeit-Validierung** aller Eingabefelder
- ✅ **Responsive Design** für alle Geräte optimiert
- ✅ **Moderne UI/UX** mit schrägen Elementen und eleganten Animationen

## 📁 Projektstruktur

```
DVGA_Landing/
├── index.html                          # Hauptseite mit Kontaktformular
├── styles.css                          # CSS-Styling im DVAG-Design mit Animationen
├── script.js                           # JavaScript mit Firebase + EmailJS Integration
├── DVAG_logo.png  # DVAG Logo (oben links)
├── FIREBASE_SETUP.md                   # Detaillierte Firebase-Anleitung
├── EMAILJS_SETUP.md                    # Detaillierte EmailJS-Anleitung
├── GITHUB_SETUP.md                     # GitHub Repository Setup-Anleitung
├── .gitignore                          # Git Ignore-Regeln
└── README.md                           # Diese Datei
```

## 🚀 Quick Start

1. **Projekt herunterladen**
   ```bash
   git clone [repository-url]
   cd DVGA_Landing
   ```

2. **Firebase einrichten** (für Datenspeicherung)
   - Folgen Sie der Anleitung in `FIREBASE_SETUP.md`
   - Tragen Sie Ihre Firebase-Konfiguration in `script.js` ein

3. **EmailJS einrichten** (für E-Mail-Benachrichtigungen)
   - Folgen Sie der Anleitung in `EMAILJS_SETUP.md`
   - Tragen Sie Ihre EmailJS-Konfiguration in `script.js` ein
   - E-Mails gehen an: christof.didi@googlemail.com

4. **Website öffnen**
   - Öffnen Sie `index.html` in Ihrem Browser
   - Das Kontaktformular ist sofort einsatzbereit

## 🌐 GitHub Repository & Deployment

**GitHub Repository:**
- Repository: [https://github.com/Christof999/DVAG](https://github.com/Christof999/DVAG) ✅ (Bereits erstellt)
- Folgen Sie der Anleitung in `GITHUB_SETUP.md` zum Hochladen
- Automatisches Hosting über GitHub Pages möglich

➡️ **Detaillierte Anleitung:** Siehe `GITHUB_SETUP.md`

## ⚙️ Firebase-Konfiguration

**WICHTIG:** Bevor das Formular funktioniert, müssen Sie Firebase einrichten:

1. Erstellen Sie ein Firebase-Projekt
2. Aktivieren Sie die Realtime Database
3. Kopieren Sie die Konfigurationsdaten
4. Ersetzen Sie die Platzhalter in `script.js`

➡️ **Detaillierte Anleitung:** Siehe `FIREBASE_SETUP.md`

## 📧 EmailJS-Konfiguration

**WICHTIG:** Für E-Mail-Benachrichtigungen müssen Sie EmailJS einrichten:

1. Erstellen Sie einen kostenlosen EmailJS-Account
2. Konfigurieren Sie Gmail als E-Mail-Service
3. Erstellen Sie ein E-Mail-Template
4. Ersetzen Sie die Platzhalter in `script.js`

➡️ **Detaillierte Anleitung:** Siehe `EMAILJS_SETUP.md`

**E-Mail-Empfänger:** christof.didi@googlemail.com

## 🎨 Design-Features

### Farben (DVAG Corporate Design)
- **Haupt-Gold:** #D4A574 (aus DVAG Logo)
- **Gold-Akzente:** #E8C4A0, #B8956B, #F5E6D3
- **Professionelles Grau:** #6B7280, #374151
- **Heller Hintergrund:** #F9FAFB
- **Reines Weiß:** #FFFFFF

### Komponenten
- **Schräger Header** mit Gold-Gradient und DVAG-Logo
- **Animierte Portrait-Sektion** mit Hover-Effekten
- **Modernes Kontaktformular** mit Echtzeit-Validierung
- **Elegante Animationen** beim Laden und bei Interaktionen
- **Professionelle Erfolgsmeldung** mit animiertem Icon
- **Responsive Design** für alle Geräte

## 📱 Responsive Breakpoints

- **Desktop:** > 768px
- **Tablet:** 481px - 768px  
- **Mobile:** < 481px

## 📊 Datenverarbeitung

**Firebase-Speicherung:**  
Alle Kontaktanfragen werden in Firebase mit folgender Struktur gespeichert:

**E-Mail-Benachrichtigung:**  
Parallel wird eine formatierte E-Mail an christof.didi@googlemail.com gesendet.

```json
{
  "kontaktanfragen": {
    "uniqueId": {
      "name": "Kundenname",
      "email": "kunde@email.de",
      "phone": "+49 123 456 7890",
      "message": "Nachricht des Kunden",
      "timestamp": "2024-01-15T10:30:00.000Z",
      "date": "15.01.2024",
      "time": "10:30:00",
      "status": "neu",
      "bearbeiter": "Vaathulan Perinparajah"
    }
  }
}
```

## 🛡️ Validierung

Das Formular validiert automatisch:
- **Name:** Mindestens 2 Zeichen
- **E-Mail:** Gültiges E-Mail-Format
- **Telefon:** Deutsche Telefonnummer-Formate
- **Nachricht:** Mindestens 10 Zeichen
- **Datenschutz:** Zustimmung erforderlich

## 🔧 Anpassungen

### Portrait-Bild ändern
Ersetzen Sie in `index.html` Zeile 18 die Platzhalter-URL:
```html
<img src="pfad/zum/ihrem/bild.jpg" alt="Vaathulan Perinparajah">
```

### Firmenfarben anpassen
Ändern Sie die CSS-Variablen in `styles.css`:
```css
:root {
    --primary-color: #FFD700;    /* Gold */
    --secondary-color: #000000;  /* Schwarz */
}
```

### Zusätzliche Felder hinzufügen
1. HTML-Feld in `index.html` einfügen
2. Validierung in `script.js` ergänzen
3. Styling in `styles.css` anpassen

## 📞 Support

Bei Fragen oder Problemen:
- **Firebase-Setup:** Siehe `FIREBASE_SETUP.md`
- **Design-Anpassungen:** Kontaktieren Sie den Entwickler
- **Technische Probleme:** Browser-Konsole prüfen

## 📄 Lizenz

Erstellt für Vaathulan Perinparajah - Deutsche Vermögensberatung AG  
© 2026 - Alle Rechte vorbehalten

---

**Version:** 1.0  
**Erstellt:** November 2024 (aktualisiert 2026)  
**Entwickelt für:** Vaathulan Perinparajah, Vermögensberater DVAG
