# Cockpit – Update-Pakete

Hier liegen die signierten Programm-Updates des Cockpit (CRM für Finanzdienstleister) der Daumann GmbH.

- `latest.json` – die neueste Version: Version, Baudatum, Hinweise, Download-Adresse und SHA-256 je Paket
- `versionen.json` – alle veröffentlichten Versionen
- `pakete/<Version>/` – `Cockpit-Update-<v>.zip.enc` (Update für alle Ausgaben, verschlüsselt), `PRUEFSUMMEN.txt`,
  `WAS-IST-NEU.md`, `version.json`

Ein Cockpit mit eingetragener Update-Quelle prüft täglich `latest.json` und bietet neuere Versionen innerhalb der
Wartung zum Einspielen an. Die Pakete sind mit einem Schlüssel verschlüsselt, den nur installierte Cockpits kennen,
und zusätzlich mit dem Händlerschlüssel signiert; das Programm prüft Signatur und Prüfsummen und lehnt veränderte
oder fremde Pakete ab. Quelltext und Erstinstallations-Pakete liegen nicht hier – die gibt es vom Hersteller.
