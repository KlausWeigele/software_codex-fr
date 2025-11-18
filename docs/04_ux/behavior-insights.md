# Behavior Insights – Motivation × Ability × Prompt

Ziel: Die Kernflows der Plattform so gestalten, dass sie mit minimaler Reibung (Ability↑) auch bei schwankender Motivation zuverlässig ausgelöst werden (Prompt), gemäß Fogg Behavior Model.

## Prinzipien
- Friction first: Jede Kernaktion in ≤2 Minuten oder ≤5 Interaktionen.
- Tiny First Step: Winzige Ersthandlung („Interesse bekunden“, „Entwurf speichern“).
- Prompting: Sofort‑, zeit‑ und ereignisbasierte Auslöser (Digest, Verfügbarkeit‑Ping, „neues Match“).
- Celebration: Sofortige positive Rückmeldung (Badge/Animation/Progress), nächstbeste Aktion vorschlagen.

## Mapping auf Flows
- Freelancer (Bewerbung)
  - Ability: LinkedIn/GitHub Import, AI‑Anschreiben, 1‑Klick „Interesse“.
  - Prompt: Daily Match‑Digest um 8:30; Ereignis „neues relevantes Projekt“.
  - Tiny: „Interesse“ statt Vollbewerbung; Verifizierung später.
- Firmen (Projektentwurf → Shortlist)
  - Ability: Project‑Builder mit 6 Feldern; AI‑Scope/ACs; Default Trial‑Week.
  - Prompt: „3 Vorschläge bereit“ nach Entwurf; Reminder 24 h ohne Aktion.
  - Tiny: Entwurf speichern → Shortlist trotzdem anzeigen.

## Experimente (30 Tage)
1) 2‑Min‑Profil vs. Standard (Freelancer)
   - Metriken: Aktivierung (Profil >60 %), `time_to_first_application`, Drop‑off‑Felder.
2) AI‑Anschreiben an/aus (Freelancer)
   - Metriken: Bewerbungs‑Abschlussrate, Bearbeitungszeit, Qualitätssignale (Antwortquote).
3) Erstprojektrabatt (0 % auf 1.000 €) vs. Trial‑Week (Firmen)
   - Metriken: Projekt‑Post‑Rate, Shortlist‑Öffnung, Deal‑Room‑Rate, Conversion zu Start.
4) Digest‑Timing 8:30 vs. 12:00 (Freelancer)
   - Metriken: CTR, Bewerbungen innerhalb 24 h, `time_to_first_action`.
5) Social Proof an/aus (Firmen)
   - Metriken: Deal‑Room‑Öffnungsrate, Startquote, Entscheidungszeit.

## Wenn‑Dann‑Pläne (Prompts)
- Freelancer: „Wenn Kaffee fertig, dann 1 Bewerbung/Interesse.“
- Firmen: „Nach Sprint‑Review freitags Shortlist prüfen (3 Kandidaten).“

## Akzeptanzkriterien (global)
- Friction‑Budget eingehalten (≤2 Min oder ≤5 Interaktionen; Abschluss ≥70 %).
- Telemetrie vollständig (`time_to_shortlist`, `completion_rate`, `field_dropoff`).
- Erfolgs‑/Fehlerzustände klar; nächste Aktion vorgeschlagen.

