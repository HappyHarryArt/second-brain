# Second Brain

Ein privates, durchsuchbares Gedächtnis auf dem eigenen Rechner. 100 % lokal, ohne Cloud,
ohne Konten, ohne laufende Kosten. Aufgebaut per Kopier-Prompt mit einem KI-Coding-Assistenten,
der auf dem Rechner Dateien anlegen und Befehle ausführen darf (Claude Code, Codex CLI,
Gemini CLI, Cursor, Aider). Ein reiner Chat im Browser reicht dafür nicht.

Live-Fassung: https://dons-dairy.okoma.app/second-brain

## Was hier liegt

- `index.html` und die verlinkten Seiten: die Anleitung in drei Stufen (Aufbauen, Füttern,
  Ausbauen) plus Referenz. Entpacken, `index.html` im Browser öffnen, fertig.
- `starterpaket/`: der Installations-Prompt (`PROMPT.md`), die Startseite mit Kopierknopf
  (`start.html`) und das Anwender-README. Dasselbe als `memory-system-paket.zip`.
- `LICENSE`: MIT-0.

## Was das System kann

SQLite mit Vektorsuche und Volltext, Einbettungen lokal über Ollama, ein Wächter für den
Eingangsordner, eine kleine Web-Oberfläche, optional ein MCP-Server, damit der eigene
KI-Assistent direkt im Gedächtnis nachschlagen kann. Die Prompts der Ausbaustufen bauen darauf
auf: Erdungsregeln gegen Halluzinationen, Ethik und Haltung, Sprach-Tagebuch, Datei-Butler,
stärkere Denk-Modelle, Fernzugriff, Buchwerkstatt.

## Lizenz

MIT No Attribution (MIT-0): benutzen, verändern, weitergeben, auch kommerziell. Namensnennung
willkommen, nicht nötig. Volker Haigis aka Don Harry, Hamburg.
