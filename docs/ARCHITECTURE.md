# Architektur

## Beobachteter Stand

Zum Zeitpunkt der Bestandsaufnahme besteht das Repository nur aus einer kurzen README-Notiz. Es gibt keinen Anwendungscode, keine festgelegte Sprache oder Frameworks, keine Build- oder Testkonfiguration und keine Deployment- oder Persistenzschicht. Die genaue Inventur steht in [CURRENT_STATE.md](CURRENT_STATE.md).

Da kein Code vorliegt, lässt sich keine bestehende technische Architektur beschreiben. Die folgenden Grenzen sind **zukünftige Architekturüberlegungen**, keine vorhandenen Module und keine verbindliche Technologieauswahl.

## Mögliche Verantwortungsgrenzen

- **Frontend:** Benutzeroberfläche und Eingaben; sollte nicht allein über kritische Spielzustände entscheiden.
- **Rendering:** Darstellung von Welt, Charakteren und Aktionen getrennt von Regeln und Datenhaltung.
- **Game Rules:** Deterministische Regeln und Validierung von Aktionen, unabhängig von UI- und KI-Text.
- **Simulation:** Optionale Systeme für Weltzeit, NPC-Verhalten und längerfristige Entwicklungen.
- **World State:** Definierte, nachvollziehbare Zustandsmodelle und Ereignisse.
- **Multiplayer:** Identitätsprüfung, Zugriffskontrolle, Synchronisierung und Konfliktbehandlung.
- **Persistence:** Reproduzierbares Speichern und Laden sowie ein migrationsfähiges Datenformat.
- **AI Orchestration:** Begrenzte Kontextbereitstellung und Verarbeitung strukturierter Modellantworten; keine direkte Autorität über Spielzustände.

Ob diese Verantwortlichkeiten in getrennten Diensten, Modulen oder einer gemeinsamen Anwendung umgesetzt werden, sollte erst nach Import und Untersuchung des Prototyps entschieden werden.

## Vertrauensgrenzen und Qualitätsziele

Kritische Aktionen müssen unabhängig von nicht vertrauenswürdigen Client-Eingaben und KI-Ausgaben validiert werden. Zugriffsrechte, Identität, persistente Änderungen und Nutzung möglicher Modell-APIs sind zu kontrollieren. Für Regeln sind gezielte Unit-Tests und für Speicherung, Synchronisierung und KI-Grenzen geeignete Integrationstests vorzusehen, sobald entsprechende Systeme existieren.

## Game: Creation

Es besteht keine technische Abhängigkeit. Eine mögliche gemeinsame Simulationsarchitektur ist lediglich eine Zukunftsoption und wird in [INTEGRATION_GAME_CREATION.md](INTEGRATION_GAME_CREATION.md) beschrieben.
