# Entwicklungsworkflow

## Ausgangspunkt

Das Repository enthält derzeit keine Anwendung und keinen nachweisbaren AI-Studio-Sync. Der Workflow ist daher eine Empfehlung für die künftige Zusammenarbeit und ersetzt keine tatsächlich vorhandenen Projektbefehle. Nach dem Prototyp-Import muss er anhand der realen Werkzeuge aktualisiert werden.

## Google AI Studio

1. Vor Änderungen prüfen, welcher Commit beziehungsweise Branch die gemeinsame versionierte Grundlage bildet.
2. Änderungen in AI Studio nicht gleichzeitig unkoordiniert mit Änderungen derselben Dateien auf GitHub bearbeiten.
3. Vor dem Export beziehungsweise Sync Änderungen sichern und nachvollziehbar einem Branch zuordnen.
4. Zugangsdaten und andere Geheimnisse nicht in Quellcode, Commits oder Dokumentation aufnehmen.
5. Den synchronisierten Stand lokal prüfen und Unterschiede zum GitHub-Branch kontrollieren.

## GitHub und GitHub Copilot

1. Pro Aufgabe einen separaten Branch verwenden.
2. Vor Änderungen README, [CURRENT_STATE.md](CURRENT_STATE.md) und [ARCHITECTURE.md](ARCHITECTURE.md) sowie passende Projektkonventionen lesen.
3. Bestehende Prototypdateien bearbeiten statt eine Ersatzanwendung zu erzeugen.
4. Kleine, fokussierte Änderungen vornehmen und relevante Dokumentation aktualisieren.
5. Pull Requests gegen die gemeinsame Basis erstellen und tatsächliche Tests transparent angeben.

## Lokale Entwicklung und Tests

- Vorhandene Setup- und Testanweisungen aus dem importierten Projekt verwenden; derzeit gibt es keine bekannten Befehle.
- Änderungen lokal prüfen, bevor sie in einen Pull Request eingehen.
- Kritische Regelmechaniken mit Unit-Tests absichern; Persistenz, Zugriffskontrollen, Synchronisierung und KI-Grenzen bei Bedarf mit Integrationstests prüfen.
- Keine Tests oder Builds als ausgeführt melden, wenn sie nicht tatsächlich durchgeführt wurden.

## Synchronisierung und Konflikte

- Nicht gleichzeitig dieselben Dateien in AI Studio und GitHub ändern.
- Änderungen über getrennte Branches und überprüfte Pull Requests zusammenführen.
- Bei Konflikten den jeweils aktuellen gemeinsamen Stand einholen, beide Änderungsabsichten prüfen und Konflikte bewusst auflösen.
- Nach einem Sync den zusammengeführten Stand erneut gegen verfügbare Tests und den Prototyp prüfen.

## Pull-Request-Prüfung

Prüfende sollten mindestens nachweisen, welche Dateien und Spielzustände betroffen sind, ob bestehende gespeicherte Spielstände erhalten bleiben, wie kritische Aktionen validiert werden und welche Tests tatsächlich liefen. Bis stabile Build- und Testbefehle aus dem Prototyp bekannt sind, werden keine automatischen CI-Befehle erfunden.
