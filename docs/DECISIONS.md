# Entscheidungen

Dieses Dokument hält Entscheidungen fest. Vorschläge und noch nicht getroffene Entscheidungen sind ausdrücklich gekennzeichnet.

## 2026-10-27 — Vorhandenen Prototyp vor Technologieentscheidungen untersuchen

- **Status:** Angenommen
- **Entscheidung:** Keine neue Anwendung, Game-Engine oder Framework-Struktur auf Grundlage von Annahmen erzeugen. Zuerst den bestehenden Google-AI-Studio-Prototyp sichern und untersuchen.
- **Begründung:** Das Repository enthält keinen Anwendungscode; der externe Prototyp wurde im Projektauftrag genannt, lag aber für die Bestandsaufnahme nicht vor.
- **Alternativen:** Einen unabhängigen Beispielprototyp oder eine vorab gewählte Technologie neu erstellen.
- **Konsequenzen:** Ein lokaler Start ist derzeit nicht möglich. Technologie- und Architekturentscheidungen bleiben offen, bis der Prototyp geprüft wurde.

## 2026-10-27 — Regeln und KI-Ausgaben getrennt halten

- **Status:** Grundsatz angenommen; technische Umsetzung offen
- **Entscheidung:** KI soll kreative Vorschläge und flexible Reaktionen unterstützen, aber nicht ungeprüft verbindliche Regeln oder Zustandsänderungen ausführen.
- **Begründung:** Spielzustände sollen deterministisch, validiert und nachvollziehbar bleiben.
- **Alternativen:** Modellantworten unmittelbar als Spielaktionen übernehmen.
- **Konsequenzen:** Spätere Architektur muss eine Validierungsgrenze zwischen KI-Ausgabe und verbindlicher Spielmechanik vorsehen.

## 2026-10-27 — Game: Creation bleibt unabhängig

- **Status:** Angenommen
- **Entscheidung:** Keine technische Abhängigkeit und kein Codeaustausch mit Game: Creation im initialen Arbeitsumfang. Mögliche gemeinsame Schnittstellen sind unverbindliche Zukunftsoptionen.
- **Begründung:** Esylium konzentriert sich auf die individuelle Rollenspielperspektive; Game: Creation auf autonome gesellschaftliche Entwicklung und strategische Simulation.
- **Alternativen:** Gemeinsame Implementierung oder direkte Abhängigkeit von Beginn an.
- **Konsequenzen:** Eine spätere Integration erfordert eine separate Architekturentscheidung.
