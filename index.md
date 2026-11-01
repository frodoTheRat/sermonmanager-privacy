---
layout: default
title: Datenschutzerklärung – SermonManager
---

# Datenschutzerklärung – SermonManager

Stand: 1. November 2026

## Kurzfassung

SermonManager ist eine App für Windows, Android und iOS zur Planung von Predigten und Gottesdiensten. **Die App sammelt, speichert und übermittelt keine Daten an den Entwickler oder an Dritte.** Alle Daten, die du in der App erfasst, bleiben auf deinem Gerät. Einzige Ausnahme ist ein optionaler, von dir ausgelöster Download von Modelldateien für die Transkription unter Windows (siehe unten); dabei werden keine Inhalte von dir übertragen.

## Verantwortlicher

Daniel Penner
E-Mail: danpen777@googlemail.com

## Welche Daten verarbeitet die App?

Die App speichert ausschließlich die Daten, die du selbst eingibst, in einer lokalen Datenbank auf deinem Gerät:

- Prediger (Name, Telefonnummer) und ihre Qualifikation für Predigt-Positionen
- Gottesdienste, Planungen und Predigten (Datum, Art, Thema, Zuordnung der Prediger)
- Unter Windows, wenn du die Transkription nutzt: der Pfad zur Aufnahme einer Predigt und der daraus erstellte Text (Transkript)
- Einstellungen der App

Die Datenbank liegt unter Windows im Ordner `%LOCALAPPDATA%\SermonManager` (bei der Installation über den Microsoft Store) bzw. neben der Programmdatei (bei der Zip-Variante), auf Android und iOS im privaten App-Speicher, auf den andere Apps keinen Zugriff haben. Der Entwickler hat auf diese Daten keinen Zugriff.

Enthält die Datenbank personenbezogene Daten Dritter (z. B. Namen und Telefonnummern von Predigern), bist du bzw. deine Gemeinde dafür verantwortlich, dass du diese Daten verarbeiten darfst und die Betroffenen informiert sind. Der Entwickler ist weder Auftragsverarbeiter noch Empfänger dieser Daten.

## Was die App nicht tut

- Keine Benutzerkonten und keine Anmeldung
- Keine Analyse-, Tracking- oder Absturzberichts-Dienste, keine Werbung
- Keine Verbindung zu Servern des Entwicklers. Alle Programmbestandteile, auch die Symbolschrift der Oberfläche, werden lokal mitgeliefert. Verbindungen zu Servern Dritter gibt es nur beim optionalen Modell-Download (siehe unten).
- Keine Weitergabe von Daten

## Transkription und Vorschläge (optional, Windows)

Unter *Einstellungen → Module* kannst du die Transkription von Predigtaufnahmen und Vorschläge für Titel, Thema, Bibelstelle und Zusammenfassung einschalten. Beides ist zunächst ausgeschaltet.

- **Verarbeitung nur auf deinem Gerät:** Die Aufnahme wird lokal von einem Spracherkennungsmodell in Text umgewandelt, und die Vorschläge erstellt ein lokales Sprachmodell aus diesem Text. Aufnahme, Transkript und Vorschläge verlassen dein Gerät nicht. Das Transkript wird in der lokalen Datenbank gespeichert und mit der Predigt gelöscht.
- **Modell-Download:** Die dafür nötigen Modelldateien sind nicht in der App enthalten. Erst wenn du in den Einstellungen auf „Herunterladen“ klickst und bestätigst, lädt die App die gewählte Datei von **Hugging Face** (`huggingface.co`, Hugging Face, Inc., USA) herunter. Dabei erhält Hugging Face wie bei jedem Download technische Verbindungsdaten, insbesondere deine IP-Adresse, Datum und Uhrzeit sowie die Kennung „SermonManager“ der App. Es werden keine Inhalte, Aufnahmen oder Daten aus der App übertragen. Für die Verarbeitung durch Hugging Face gilt dessen Datenschutzerklärung (<https://huggingface.co/privacy>). Alternativ kannst du eine Modelldatei, die du selbst beschafft hast, über „Importieren“ übernehmen; dann findet keine Verbindung statt.
- **Speicherort:** Die Modelldateien liegen im Ordner `%LOCALAPPDATA%\SermonManager\models` und können dort oder in den Einstellungen jederzeit gelöscht werden.

## Lokaler Webserver (Windows)

Die Windows-Version zeigt ihre Oberfläche über einen kleinen Webserver an, der ausschließlich auf deinem Gerät läuft (Adresse `127.0.0.1`, zufälliger Port). Er ist aus dem Netzwerk oder dem Internet nicht erreichbar.

## Protokolldateien

Die App schreibt technische Protokolle (z. B. Fehlermeldungen) in einen Ordner `logs` neben der Datenbank (auf Android und iOS im privaten App-Speicher). Sie verlassen dein Gerät nicht. Du kannst sie jederzeit löschen.

## Exportierte Dateien

Wenn du eine Predigerliste als Excel-, Word- oder PDF-Datei exportierst, speicherst du die Datei an einem Ort deiner Wahl. Auf Android und iOS öffnet die App dafür das Teilen-Menü deines Geräts; die Datei geht erst an die App, die du dort auswählst. Was du mit der Datei machst, entscheidest allein du.

## Komponenten von Microsoft

Zur Darstellung der Oberfläche nutzt die App die **Microsoft Edge WebView2 Runtime**, eine Komponente von Microsoft, die auf deinem Gerät installiert ist. Für diese Komponente und für den Microsoft Store gelten die Datenschutzbestimmungen von Microsoft (<https://privacy.microsoft.com>). Der Entwickler hat darauf keinen Einfluss. Die lokalen Browserdaten dieser Komponente (z. B. Zwischenspeicher) liegen im Ordner `%LOCALAPPDATA%\SermonManager\WebView2`.

## Komponenten von Google und Apple (Android, iOS)

Zur Darstellung der Oberfläche nutzt die App die in dein Gerät integrierte Web-Ansicht (Android System WebView bzw. WKWebView von Apple). Für diese Systemkomponenten und für den Google Play Store bzw. den App Store gelten die Datenschutzbestimmungen von Google bzw. Apple. Der Entwickler hat darauf keinen Einfluss.

## Gerätesicherung (Android, iOS)

Die Datensicherung deines Geräts (Google-Backup unter Android, iCloud-Backup unter iOS) kann die App-Daten einschließen, wenn du diese Sicherung in den Systemeinstellungen aktiviert hast. Das geschieht durch das Betriebssystem, nicht durch die App; der Entwickler erhält diese Daten nicht. Du kannst die Sicherung in den Einstellungen deines Geräts abschalten.

## Löschen deiner Daten

- **Microsoft Store:** Beim Deinstallieren der App werden ihre Daten vom Gerät entfernt. Die Datenbank kannst du auch jederzeit manuell löschen, ebenso heruntergeladene Modelle im Ordner `models`.
- **Zip-Variante:** Lösche den Programmordner samt `sermonManager.db` und gegebenenfalls den Ordner `%LOCALAPPDATA%\SermonManager\models`.
- **Android und iOS:** Deinstalliere die App oder lösche in den Systemeinstellungen den Speicher der App; damit werden Datenbank und Protokolle entfernt.

Sichere deine Daten selbst, wenn du sie behalten willst (unter Windows: kopiere die Datei `sermonManager.db` an einen sicheren Ort).

## Kinder

Die App richtet sich nicht an Kinder und erhebt keine Daten von ihnen.

## Änderungen dieser Erklärung

Wenn sich die Funktionen der App ändern, wird diese Erklärung angepasst. Die jeweils aktuelle Fassung findest du unter der Adresse, unter der du sie gerade liest.

## Kontakt

Bei Fragen zum Datenschutz erreichst du mich unter danpen777@googlemail.com.
