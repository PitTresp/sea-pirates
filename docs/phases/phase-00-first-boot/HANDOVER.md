Phase 0 → Phase 1 Handover
Übergabe

Von: Phase 0 – The First Boot
Nach: Phase 1 – Everything is an Object
Status: Phase 0 abgeschlossen

Ausgangsziel

Phase 0 sollte eine reproduzierbare und nachvollziehbare technische sowie dokumentarische Ausgangsbasis für SEA Pirates herstellen.

Es sollten ausdrücklich noch keine fachlichen Features der SEA Academy und keine vorweggenommene Produktarchitektur implementiert werden.

Erreichter technischer Stand

Entwicklungsumgebung:

Visual Studio Community 2022 17.14.37
C#-Werkzeuge installiert
.NET SDK 9.0.316
Git 2.54.0

Repository:

GitHub-Repository sea-pirates
Branch main
lokales Repository mit origin/main verbunden
.gitignore für IDE-, Build- und lokale Artefakte eingerichtet

.NET:

SeaPirates.sln im Repository-Root
src/SeaPirates/SeaPirates.csproj
Target Framework net9.0
Console Application als bewusst minimale Ausgangsbasis
Project der Solution hinzugefügt
dotnet run erfolgreich
dotnet build SeaPirates.sln erfolgreich
Repository-Grundstruktur
sea-pirates/
├── AI-START.md
├── README.md
├── MANIFEST.md
├── PROJECT-STATE.md
├── SeaPirates.sln
├── docs/
│   ├── LEARNING-ROADMAP.md
│   └── phases/
│       └── phase-00-first-boot/
│           ├── README.md
│           └── HANDOVER.md
├── exercises/
└── src/
    └── SeaPirates/
        ├── SeaPirates.csproj
        └── Program.cs

Leere Verzeichnisse müssen nicht zwangsläufig durch Git versioniert sein.

Erarbeitete Grundlagen
Git

Git-Grundlagen sind bereits aus vorheriger Projektarbeit bekannt und sollen nicht unnötig erneut trainiert werden.

Bekannt sind unter anderem:

Working Tree
Staging Area
Commit
Push/Pull
Remote / origin
git status
git diff
git diff --cached
git log --oneline

Git wird weiterhin praktisch verwendet. Vertiefungen erfolgen bei neuen Themen oder konkretem Bedarf.

.NET

Erarbeitet wurde das grundlegende Modell:

C#-Quellcode
    ↓
C#-Compiler
    ↓
IL
    ↓
Assembly
    ↓
.NET Runtime / JIT
    ↓
Maschinencode
    ↓
CPU

Das Modell ist bewusst vereinfacht.

CLR-, JIT-, Assembly- und Build-Details werden bei praktischem Bedarf vertieft.

Solution und Project

Verstanden wurde:

Eine Solution organisiert zusammengehörige Projects.
Ein Project ist eine eigenständig baubare Einheit.
Eine Solution kann mehrere Projects enthalten.
Ein Project kann grundsätzlich ohne Solution existieren und gebaut werden.
.csproj beschreibt die Konfiguration eines C#-Projects.

Beispiel für eine mögliche spätere Struktur:

SeaPirates.sln
├── SeaPirates.App.csproj
├── SeaPirates.Api.csproj
└── SeaPirates.Tests.csproj

Diese Struktur ist nur ein Verständnisbeispiel und keine Architekturentscheidung für SEA Academy.

Build-Artefakte

Verstanden wurde:

bin/ enthält primär Build-Ausgaben.
obj/ enthält Zwischenartefakte des Build-Prozesses.
beide sind reproduzierbar und werden deshalb nicht regulär versioniert.
Lernstand

Der Lernende kann aktuell bereits grundlegende OOP-Begriffe teilweise erklären.

Vor Phase 0 wurden unter anderem diskutiert:

Vererbung
Komposition
ist-ein-Beziehung
hat-ein-Beziehung
„Composition over Inheritance“

Dabei wurde erkannt, dass das reine Erkennen einer sprachlich möglichen ist-ein-Beziehung noch nicht automatisch bedeutet, dass Vererbung die beste Modellierungsentscheidung ist.

Diese Themen sind noch nicht abgeschlossen und werden in den kommenden OOP-Phasen systematisch praktisch aufgebaut.

Lernpräferenz

Freie Lösungsfindung ist ausdrücklich erwünscht.

Der Lernende möchte:

zunächst selbst überlegen,
Fehler machen dürfen,
Entscheidungen begründen,
Hintergründe verstehen,
zunehmend komplexeren Code lesen,
Fachbegriffe mit praktischem Verständnis verbinden.

Fertige Lösungen sollen nicht unnötig vorweggenommen werden.

Produktkontext

Als durchgängiges Praxisprojekt entsteht die SEA Academy.

Zielbild ist ein wachsendes Wissens- und Lernmanagementsystem.

Mögliche spätere Inhalte sind beispielsweise:

Lerninhalte,
Fragen,
Notizen,
Codebeispiele,
Kategorien,
Übungen,
Lernstände.

Diese Punkte sind noch keine vollständigen Anforderungen.

Die Anwendung soll organisch mit den Lerninhalten wachsen.

Nicht entschieden

Noch nicht festgelegt sind insbesondere:

endgültige Produktarchitektur
Datenbank
Persistenztechnologie
Web-Framework
Benutzeroberfläche
API-Architektur
Repository Pattern
Dependency-Injection-Struktur
konkrete Design Patterns

Diese Entscheidungen dürfen nicht aus Gewohnheit oder vorsorglich getroffen werden.

Einstieg Phase 1

Nächste Phase:

Phase 1 – Everything is an Object

Schwerpunkte:

Klasse
Objekt
Felder
Properties
Methoden
Konstruktoren
Sichtbarkeit
Kapselung
Referenzen
erste systematische Codeanalyse

Der Einstieg soll über ein kleines eigenes Domänenobjekt der SEA Academy erfolgen.

Nicht mit einer fertigen Klassenhierarchie beginnen.

Der Lernende soll zunächst selbst überlegen:

Welches reale oder fachliche Konzept wollen wir als erstes Objekt modellieren und welche Verantwortung sollte dieses Objekt besitzen?

Von dort wird der Code schrittweise aufgebaut.

Phase-1-Leitplanke

Noch keine unnötigen:

Interfaces
Services
Repositories
Datenbanken
Frameworks
Design Patterns

Phase 1 soll das Fundament von Klassen und Objekten herstellen.

Komplexität wird erst hinzugefügt, wenn der Lernfortschritt oder ein konkret auftretendes Problem sie rechtfertigt.

Übergabeentscheidung

Phase 0 ist bereit zur Übergabe an Phase 1.