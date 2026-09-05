# Persönliches Lokales Gedächtnis (RAG) — Starterpaket

*Paket-Stand: Juli 2026 (v2 — Komfort-Interface mit Dialog, Drag & Drop, „Merk dir das“ und Export).*

Vorgestellt im Vibe Coding Club Hamburg.

Dieses Paket installiert dir ein **komplett lokales, privates
Gedächtnis-System** ("Second Brain") auf deinem Rechner — Mac oder Windows.
Deine Notizen und Dokumente bleiben zu 100 % auf deinem Gerät.
Keine Cloud, keine Konten, keine Kosten.

---

## Was ist in diesem Paket?

| Datei       | Zweck                                                        |
|-------------|--------------------------------------------------------------|
| `start.html`| Anleitung zum Öffnen im Browser — mit Kopier-Button für den Prompt |
| `PROMPT.md` | Der eigentliche Installations-Prompt für Claude Code          |
| `README.md` | Diese Datei                                                   |

---

## Was du vorher brauchst (einmalig)

**Claude Code** — das ist die einzige Voraussetzung.

1. Gehe auf https://claude.com/claude-code und folge der
   Installationsanleitung für dein Betriebssystem.
2. Du brauchst ein Claude-Konto (Pro-Abo oder API-Zugang).

Alles andere — Ollama, Python, das Embedding-Modell — installiert
Claude Code für dich und **fragt dich vor jedem Schritt um Erlaubnis**.

---

## Installation in 3 Schritten

1. **Öffne `start.html`** in deinem Browser (Doppelklick).
2. **Klicke auf "Prompt kopieren"** — der komplette Installations-Prompt
   liegt jetzt in deiner Zwischenablage.
3. **Öffne ein Terminal, starte `claude`** und füge den Prompt ein
   (Cmd+V auf dem Mac, Strg+V unter Windows). Enter drücken.

Claude Code führt dich nun Schritt für Schritt durch die Installation
und erklärt jeden Schritt in einfacher Sprache. Du musst nur bestätigen.

Dauer: ca. 10–15 Minuten (inkl. ~270 MB Modell-Download).

---

## Was am Ende auf deinem Rechner läuft

```
Web-Oberfläche (http://localhost:8600)
        ↓
FastAPI-Server (Python)
        ↓
SQLite-Datenbank (eine einzige Datei = dein Gedächtnis)
        ↓
Ollama (lokale KI für Embeddings, optional Antworten)
```

**So benutzt du es täglich:**

- **Fragen (Dialog):** Öffne http://localhost:8600 und frag einfach —
  die Antwort kommt als Gespräch, mit den Fundstellen darunter.
- **Erinnerungen hinzufügen:** Dateien (Markdown, Text, PDF) einfach
  **per Drag & Drop** auf die Oberfläche ziehen — oder in den Ordner
  `~/memory/inbox/` legen. Kurze Gedanken: ins Feld tippen und
  **„Merk dir das“** drücken.
- **Exportieren:** Antwort oder ganzes Gespräch als sauberes
  HTML-Dokument sichern — über den Druck-Dialog wird daraus ein PDF
  oder ein einfaches Handout.
- **Starten:** Doppelklick auf `start.command` (Mac) bzw. `start.bat`
  (Windows) im Ordner `~/memory-system/`.
- **Backup:** Sichere einfach die eine SQLite-Datei. Fertig.

---

## Später anpassen (Vibe Coding!)

Die Web-Oberfläche ist eine einzige, ausführlich kommentierte HTML-Datei.
Öffne den Ordner `~/memory-system/` in Claude Code oder Cursor und sag
einfach, was du willst:

- "Mach mir einen Dark Mode"
- "Füge Tags für meine Notizen hinzu"
- "Zeige die neuesten Erinnerungen auf der Startseite"

Genau dafür ist das System gebaut: klein, lesbar, deins.

---

## Häufige Fragen

**Verlässt irgendetwas meinen Rechner?**
Nein. Embeddings und Suche laufen lokal über Ollama. Nur die Installation
selbst (über Claude Code) nutzt die Claude-API.

**Was kostet das?**
Das System selbst: nichts. Claude Code benötigt ein Claude-Abo,
das viele im Club ohnehin haben.

**Wie viel Speicherplatz?**
Ollama + Embedding-Modell: ca. 1 GB. Die Datenbank wächst mit deinen
Notizen, bleibt aber typischerweise unter 100 MB.

**Kann mein KI-Assistent auf mein Gedächtnis zugreifen?**
Ja — die Installation richtet optional einen MCP-Server ein. Dann kann jeder
MCP-fähige Assistent (Claude Code, Claude Desktop, Cursor, Codex CLI, Gemini CLI,
ChatGPT Desktop) direkt in deinen Erinnerungen nachschlagen.
