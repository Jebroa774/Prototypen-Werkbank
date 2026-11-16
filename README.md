# Prototypen-Werkbank

Eine lokale Windows-App für Prototypen: Pinbelegungen, erkennbare Bauteilansichten, Verdrahtung, Stücklisten, Lager, Messprotokolle und Entwicklungsnotizen an einem Ort.

[Windows-App herunterladen](https://github.com/Jebroa774/Prototypen-Werkbank/releases/latest/download/Prototypen-Werkbank-Windows.zip)

## Installieren

1. Die ZIP-Datei vollständig entpacken.
2. `Installieren.exe` doppelt anklicken. Die Installation erfolgt im eigenen Benutzerprofil und benötigt keine Administratorrechte.
3. Anschließend die Werkbank über das Desktop- oder Startmenü-Symbol öffnen.

Benötigt werden Windows 10/11 mit x64-Unterstützung und Microsoft Edge. Die Node-Laufzeit liegt bereits im Paket.

## Automatische Updates

Bei jedem App-Start wird der öffentliche HTTPS-Updatekanal geprüft. Neuere Versionen werden anhand des im Installer hinterlegten Ed25519-Schlüssels und ihrer SHA-256-Prüfsummen geprüft und automatisch installiert. Vorher wird die lokale Datenbank gesichert. Ohne Internet startet die vorhandene Version; bei einem fehlgeschlagenen Update-Start wird die vorherige Appversion wiederhergestellt.

Unter **Diagnose & Updates** lässt sich der aktuelle Stand auch bei laufender App prüfen. Ein verfügbares Update wird beim nächsten App-Start übernommen.

## Eigene Projekte und weitere PCs

Eine neue Installation beginnt ohne persönliche Projekte. Zum Umziehen auf einen weiteren PC in der alten Werkbank **Sicherung exportieren** wählen und die JSON-Datei auf dem neuen PC mit **Sicherung importieren** einlesen. Anschließend beziehen beide Installationen ihre App-Updates unabhängig von diesem öffentlichen Kanal.

Projekte, Datenbanken, Repository- und Chat-Importe sowie Diagnose-Logs werden weder in diesem Repository veröffentlicht noch automatisch hochgeladen. Die App speichert ihre Projektdaten lokal. Persönliche Projekte werden nicht zwischen Geräten synchronisiert.

## Funktionen

- Projekte mit Firmwarestand, Pinbelegung, Bauteilen und Prüfliste.
- Zoombare 2D-Bauteilansichten, Verdrahtung und SVG-Export.
- Manuelle Verdrahtungsprüfung, die Änderungen an Anschlüssen berücksichtigt.
- Laborjournal für Messwerte, Änderungen, Fehler und Notizen.
- Lagerbestände, Bestellungen, Fehlteilliste, Lagerorte und Datenblattlinks.
- Offline-Projektberichte zum Lesen und Drucken sowie CSV-Exporte.
- Rechenhilfen für Ohmsches Gesetz und unbelastete Spannungsteiler.
- USB-Gerätestatus und SSH-Verknüpfungen zu selbst eingetragenen Geräten.
- Lokale, begrenzte Diagnose-Logs mit Export zum Weitergeben bei Fehlern.

Die Lizenztexte der mitgelieferten Node-Laufzeit und ihrer Bibliotheken liegen im Paket unter `App-Paket/runtime/node-LICENSE.txt`.
