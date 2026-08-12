# SEA Pirates – Project State

## Aktuelle Phase

**Phase 0 – The First Boot**

Status: Abgeschlossen

## Ziel der Phase

Eine reproduzierbare und nachvollziehbare Ausgangsbasis für SEA Pirates
und die spätere Entwicklung der SEA Academy herstellen.

## Technischer Stand

- Visual Studio Community 2022 17.14.37
- C#-Werkzeuge verfügbar
- .NET SDK 9.0.316
- Git 2.54.0
- GitHub-Repository `sea-pirates`
- Branch `main`
- `SeaPirates.sln` im Repository-Root
- Console-Projekt `src/SeaPirates/SeaPirates.csproj`
- Target Framework `net9.0`
- Build erfolgreich
- Anwendung über `dotnet run` ausführbar

## Verstandene Grundlagen

- Unterschied zwischen IDE, .NET SDK und .NET Runtime
- Solution als Verbund zusammengehöriger Projects
- Project als eigenständig baubare Einheit
- Aufgabe der `.csproj`
- Zweck von `bin/` und `obj/`
- grundlegende Build-Kette:
  C# → IL → Assembly → JIT → Maschinencode → CPU

## Festgelegte Entscheidungen

- Hauptsprache: C#
- Plattform: .NET
- Primäre IDE: Visual Studio
- SEA Academy als kontinuierlich wachsendes Lernprojekt
- Architektur und Frameworks werden nicht vorzeitig festgelegt
- Lernen durch freie Lösungsfindung, Fehleranalyse und Reflexion
- vereinfachter, bedarfsgerechter Dokumentationsstandard

## Prüfungsziel

AP2 Fachinformatiker Anwendungsentwicklung am 25.11.2026.

Zusätzlich wird grundsätzlich eine alte Prüfung pro Woche bearbeitet,
beginnend mit der zuletzt verfügbaren Prüfung und anschließend rückwärts.

## Nächste Phase

**Phase 1 – Everything is an Object**

Geplante Themen:

- Klasse und Objekt
- Felder und Properties
- Methoden
- Konstruktoren
- Sichtbarkeit
- Kapselung
- Referenzen
- erste Codeanalyse

## Wiedereinstieg

1. `README.md` lesen, falls das Projekt unbekannt ist.
2. `PROJECT-STATE.md` lesen.
3. `docs/LEARNING-ROADMAP.md` prüfen.
4. Phase 1 mit einem ersten eigenen Domänenobjekt der SEA Academy beginnen.
5. Keine Architektur vorwegnehmen.