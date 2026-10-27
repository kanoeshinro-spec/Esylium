# Roadmap

Die Reihenfolge priorisiert zunächst die Bestandsaufnahme des externen Prototyps, da das Repository aktuell keinen ausführbaren Spielcode enthält. Phasen sind Vorschläge und können sich nach Prüfung des Imports ändern.

## 1. Prototyp sichern und technisch stabilisieren

- Den Google-AI-Studio-Prototyp reproduzierbar exportieren beziehungsweise synchronisieren und in einem separaten Branch einbringen.
- Lizenz- und Zugangsdaten prüfen; keine Geheimnisse einchecken.
- Vorhandene Technologien, Komponenten, Funktionen, Speicherung und externe Abhängigkeiten inventarisieren.
- Bestehende Start-, Build- und Testwege ermitteln und reproduzierbar machen; keine unbekannten Befehle voraussetzen.
- Änderungen an AI-Studio- und GitHub-Kopien über geprüfte Pull Requests zusammenführen.

## 2. Spielzustand und Charakter sichern

- Charakter- und Weltzustandsmodell aus dem tatsächlichen Prototyp ableiten.
- Speicher- und Ladeverhalten sowie mögliche Migrationen festlegen.
- Regeln und kritische Zustandsübergänge mit Tests absichern.

## 3. Accounts und Multiplayer-Grundlagen

- Sichere Identitätsprüfung und Zugriffskontrollen festlegen.
- Anforderungen für konsistente Synchronisierung gemeinsamer Zustände bestimmen.
- Erst danach eine passende Server- und Persistenzarchitektur auswählen.

## 4. Welt und Darstellung erweitern

- Vorhandene Rendering- und Weltkomponenten ausbauen, falls im importierten Prototyp vorhanden.
- Erweiterte Erkundung und visuelle Welt schrittweise ergänzen.

## 5. NPCs, Dialoge und KI-Spielleitung

- NPC- und Dialogverhalten definieren.
- KI-Ausgaben strukturiert begrenzen und von deterministischer Regelvalidierung trennen.
- API-Nutzung, Kontextgrenzen, Kosten und Fehlerfälle kontrollieren.

## 6. Kampf

- Taktische Regeln als testbare Mechaniken definieren.
- Aktionen gegen nicht vertrauenswürdige Eingaben validieren.

## 7. Inventar, Ressourcen und Crafting

- Inventar- und Ressourcenzustände modellieren.
- Handwerk und Wirtschaft auf validierte Zustandsänderungen stützen.

## 8. Persistente Weltsimulation

- Siedlungen, Fraktionen, Weltzeit und langfristige Ereignisse in überprüfbaren Schritten entwickeln.
- Eine mögliche Schnittstelle zu Game: Creation nur bei konkretem Bedarf und weiterhin ohne technische Abhängigkeit untersuchen.
