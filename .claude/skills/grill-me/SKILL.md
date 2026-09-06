---
name: grill-me
description: Timon vor größeren Bauvorhaben gründlich interviewen, bis nichts Wichtiges mehr offen ist, dann Spec schreiben. Nutzen bei jedem neuen Feature/Projekt/Produkt, das mehr als einen Satz Beschreibung braucht — oder wenn Timon /grill-me sagt.
---

# Grill me — Interview vor dem Bau

Zweck: Jede ungestellte Frage wird später ein Bug oder eine Fehlentwicklung. (Methode von Matt Pocock; Anthropic-Best-Practice.)

## Ablauf
1. **Erst selbst erkunden:** Wenn eine Frage durch Lesen des Codes/der Dateien/der Memories beantwortbar ist, NICHT fragen — nachschauen.
2. **Dann interviewen**, mit dem AskUserQuestion-Tool, in Runden à 2–4 Fragen (Timon diktiert — Fragen so stellen, dass kurze Antworten reichen). Themen-Baum abarbeiten, Abhängigkeiten zwischen Entscheidungen einzeln auflösen:
   - Ziel & Nutzer: Wer benutzt es, was ist der eine Job?
   - Geld/Aufwand: Was darf es kosten, wann ist es „gut genug"?
   - Daten & Anbindungen, Hosting/Betrieb, Freigabe-Grenzen (was darf es NIE allein?)
   - Aussehen/Ton, Erfolgs-Check (woran messen wir fertig?)
3. **Nicht aufhören**, solange eine Antwort neue Fragen aufwirft. Bei komplexen Vorhaben sind 15–30 Fragen normal.
4. **Abschluss:** Komplette Spec nach `SPEC.md` (bzw. Projektkonvention) schreiben: Ziel, Nutzer, Features nummeriert, Nicht-Ziele, offene Risiken, Erfolgs-Checks. Umsetzung erst NACH Timons Ok zur Spec — idealerweise in frischer Session.
