# lwb-lab

Gemeinsamer Rahmen der AG KI für KI-gestützte Projekte der Lichtenberger Werkstätten gGmbH.

## Inhaltsverzeichnis

- [Zweck dieser Organisation](#zweck-dieser-organisation)
- [Aufnahme neuer Projekte](#aufnahme-neuer-projekte)
- [Namensregeln](#namensregeln)
- [Kategorisierung über Topics](#kategorisierung-über-topics)
- [Aufbau eines Repositorys](#aufbau-eines-repositorys)
- [Verantwortlichkeiten](#verantwortlichkeiten)
- [Arbeitsablauf](#arbeitsablauf)
- [Rahmenbedingungen](#rahmenbedingungen)

## Zweck dieser Organisation

lwb-lab bündelt die gemeinsam entwickelten KI-Vorhaben der AG KI. Jedes Vorhaben erhält ein eigenes Repository mit nachvollziehbarer Änderungshistorie, klarer Verantwortung und einem geregelten Freigabeprozess. Lokale Experimente außerhalb dieser Organisation bleiben davon unberührt.

## Aufnahme neuer Projekte

Ein Vorhaben wird in lwb-lab aufgenommen, sobald

- ein betrieblicher Nutzen erkennbar ist,
- ein abgegrenztes Ziel feststeht,
- eine verantwortliche Person benannt ist.

Ein Prototyp ist dafür nicht erforderlich.

## Namensregeln

Repositorys werden nach dem Projekt benannt, nicht nach ihrem Typ. Der Name soll auch ohne Zusatzwissen erkennen lassen, worum es inhaltlich geht.

Beispiele: `apply-lwb-branding`, `Monatsstatistik`

Kein Typ-Präfix im Namen (also nicht `skill-...` oder `app-...`). Die Einordnung nach Typ erfolgt ausschließlich über Topics (siehe unten).

## Kategorisierung über Topics

Da der Name selbst keinen Rückschluss auf den Projekttyp zulässt, erhält jedes Repository mindestens ein Topic aus folgender Liste:

| Topic | Bedeutung |
|---|---|
| `skill` | Claude-Skill: wiederverwendbare Anweisungen und ggf. Dateien für eine bestimmte KI-Aufgabe |
| `project` | Eigenständige Anwendung oder Werkzeug (z. B. Web-App, Tool) |
| `docs` | Dokumentation, Konzepte, Arbeitsweisen ohne eigenen Anwendungscode |

Topics werden über die Repo-Einstellungen auf github.com gesetzt (Zahnrad-Symbol neben der Beschreibung im "About"-Bereich). Weitere Topics zur inhaltlichen Verschlagwortung (z. B. ein zweites Topic mit dem fachlichen Thema) sind zulässig, zusätzlich zur Typ-Kategorie.

Neue Topic-Kategorien werden hier ergänzt, sobald sie gebraucht werden — nicht spontan im einzelnen Repo frei vergeben.

## Aufbau eines Repositorys

Jedes Repository enthält eine eigene README mit:

- Zweck des Projekts
- Verantwortliche Person
- Dateiablage / Struktur
- Test- und Bereitstellungsanleitung

## Verantwortlichkeiten

| Rolle | Aufgabe |
|---|---|
| Administration | Marco (mit zu benennender Vertretung) — verantwortet die gemeinsamen Regeln dieser Organisation |
| Projektverantwortliche Person | Fachkundige Person je Projekt — steuert Änderungen, verantwortet die Freigabe (Merge in Main) |
| Zweitprüfung | Weiteres AG-Mitglied — prüft unabhängig vor der Freigabe |

## Arbeitsablauf

1. **Projektstand holen** — Clone beim ersten Mal, sonst Pull vor jeder neuen Aufgabe. `main` ist der gemeinsam geprüfte Hauptstand.
2. **Branch anlegen** — jede Änderung in einem eigenen Arbeitszweig, `main` bleibt unverändert.
3. **Bearbeiten und selbst testen** — Änderung mit Claude umsetzen, Ergebnis mit Beispieldaten prüfen. Eine plausible KI-Antwort allein gilt nicht als Test.
4. **Commit und Push** — nachvollziehbare Zwischenstände mit kurzer Beschreibung, dann in den Arbeitszweig hochladen.
5. **Pull Request** — Änderung, Zweck und Testergebnis beschreiben. Mindestens zwei Personen testen unabhängig.
6. **Merge** — nach erfolgreicher Zweitprüfung durch die projektverantwortliche Person. Direkte Änderungen an `main` sind nicht vorgesehen.
7. **Bereitstellung** — Skills werden zunächst als Testfassung geteilt, nach Freigabe zentral aktualisiert. Web-Apps laufen zunächst in einem Testbereich, nach Freigabe im regulären Betrieb.

## Rahmenbedingungen

- Keine personenbezogenen Daten, Zugangsdaten oder vertraulichen Unterlagen in Claude oder den Repositorys. Weitere interne Inhalte werden mit der IT abgestimmt.
- Repositorys sind zunächst privat, Zugriff wird über persönliche Konten vergeben.
- Vorherige freigegebene Versionen bleiben auffindbar, um bei Problemen gezielt zurückwechseln zu können.
