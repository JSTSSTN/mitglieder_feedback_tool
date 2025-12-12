ON STAGE Training Center – Feedback Tool

Ein responsives, interaktives Web-Feedback-Tool für das ON STAGE Training Center.
Es ermöglicht Mitgliedern (Erwachsene und Kids), strukturiertes Feedback abzugeben und sendet die Daten automatisiert an ein Google Apps Script zur Speicherung.

Das Tool eignet sich für Fitnessstudios, Tanzschulen, Vereine und andere Einrichtungen, die unkompliziert Rückmeldungen sammeln möchten.

Features
Zwei Modi: Erwachsene und Kids

Unterschiedliches Design und Farbschema

Altersgerechte Fragen

Dynamisches Umschalten des Themes

Bewertungssystem mit Sternen

1 bis 4 Sterne

Auswahl per Klick

Visuelle Hervorhebung der gewählten Sterne

Kommentarfelder

Zu jeder Frage kann optional ein Kommentar eingegeben werden

Standortauswahl

Auswahl zwischen mehreren Standorten

Verhindert unvollständige Feedbacks

Dynamisches Formular

Das Feedback-Formular wird per JavaScript generiert

Fragen basierend auf dem gewählten Modus

Automatischer Versand an Google Apps Script

POST-Request im JSON-Format

Funktioniert mit Google Sheets

no-cors Modus zur Vermeidung von CORS-Fehlern

Danke- und Fehlermeldungen

Deutliche Rückmeldung bei Erfolg oder Verbindungsfehlern

Tech Stack

HTML5

CSS3

JavaScript (Vanilla JS)

Google Apps Script (Backend)

Fetch API

Projektstruktur
/projekt
│── index.html        # Hauptdatei mit HTML, CSS und JavaScript
│── Images/           # Logos und Assets
└── README.md         # Projektdokumentation

Installation und Nutzung

Da das Projekt vollständig clientseitig ist, muss nichts installiert werden.

Lokale Nutzung

Repository herunterladen oder klonen

index.html öffnen

Das Feedback-Tool startet im Browser

Deployment

Das Tool kann auf allen gängigen Plattformen gehostet werden:
GitHub Pages, Vercel, Netlify oder jeder andere Webserver.

Backend (Google Apps Script)

Das Feedback wird an folgendes Script gesendet:

https://script.google.com/macros/s/AKfycbzEbjJMqX_MpL-kg-BzgjGRH5oO9QrlXXBm0SpS7UTK8UBUWNpd63xACS-Fz4LmZ3iqvQ/exec

Beispiel-Request:
{
  "bereich": "Kids",
  "standort": "Am Felde",
  "feedback": [
    {
      "frage": "Wie viel Spaß macht dir das Training?",
      "bewertung": "Sehr zufrieden",
      "kommentar": "Super cool!"
    }
  ]
}

Validierung und Fehlerhandling

Standort muss ausgewählt sein

Jede Frage benötigt eine Bewertung

Fehlermeldung bei Verbindungsproblemen

Während des Sendens wird der Button deaktiviert, um doppelte Einsendungen zu vermeiden

Wesentliche Code-Aspekte
Dynamische Erstellung des Formulars

Das komplette Feedback-Formular wird zur Laufzeit aus JavaScript generiert.

Klare Struktur

Getrennte Logik für Moduswahl, Bewertung, Formularerzeugung und Absenden

Fragen sind in Arrays organisiert und leicht erweiterbar

Responsives Design

Optimal nutzbar auf Desktop, Tablet und Smartphone.

Erweiterungsideen

Export als CSV oder Excel

Administrations-Dashboard zur Auswertung

Backend mit Node.js/Express

Offline-Modus

Ladeanimation während der Übermittlung

Autor

Name: Justus Stein
GitHub: https://github.com/JSTSSTN