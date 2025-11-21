# Zielbild-Template für SaaS- und AI-Produkte

Status: Entwurf v0.1  
Zweck: Wiederverwendbare Struktur, um für jede Geschäftsidee ein klares
„Target State“-Dokument zu formulieren – ähnlich wie bei der
Freelancer-Plattform, aber allgemein gehalten.

Hinweis zur Nutzung:
- Pro konkreter Idee eine Kopie dieser Datei anlegen und ausfüllen.
- Kurz und prägnant bleiben; lieber klare Bullet-Points als Romane.
- Wo möglich auf Metriken und Beispiele runterbrechen.

---

## 1. Produkt-Vision

Kurzbeschreibung in 2–4 Sätzen:
- Welches Ergebnis soll für Kund:innen am Ende stehen?
- Welche Rolle spielen Software und ggf. KI?
- Wie fühlt sich „Erfolg“ aus Sicht der Nutzer an?

---

## 2. Zielgruppen & Rollen

Wer nutzt das Produkt, wer entscheidet, wer bezahlt?
- Primäre Zielgruppen (Branche, Unternehmensgröße, Funktion).
- Wichtige Rollen/Personas (z. B. „Teamleiter X“, „Freelancer Y“).
- Welche Probleme/Jobs-to-be-done haben sie heute?

---

## 3. Leitprinzipien des Produkts

Grundsätze, an denen sich Entscheidungen orientieren:
- z. B. „AI-first, human-in-the-loop“,
- „Liberal & anreizbasiert statt restriktiv“,
- „Measurement by default“,
- „Qualität vor Masse“, „Low Friction“.

---

## 4. Problem & Pain Points

Welche konkreten Probleme adressiert das Produkt?
- 3–7 zentrale Pain Points (jeweils 2–3 Sätze).
- Warum treten diese Probleme heute auf (in diesem Markt, Land, Segment)?
- Was tun Kunden heute (Workarounds, Tools, Dienstleister)?
- Schwächen der heutigen Lösungen.

---

## 5. Wertversprechen & Differenzierung

Warum ist dieses Produkt für diese Zielgruppe wertvoll und anders?
- Kernversprechen (max. 3 Bullet-Points).
- Wie differenziert es sich von bestehenden Lösungen / Wettbewerbern?
- Welche Aspekte sind besonders wichtig in Deutschland/DACH (z. B. Sprache, Recht, Kultur)?

---

## 6. Kernfunktionen (Version 1)

Welche Funktionen braucht die erste Version wirklich?
- 3–7 Kernfunktionen, die zusammen einen „End-to-End“-Wert erzeugen.
- Für jede Funktion:
  - kurzer Zweck,
  - wichtigste Nutzeraktionen,
  - was bewusst NICHT in V1 drin ist (Non-Goals).

---

## 7. Rolle von KI (falls relevant)

Wie genau hilft KI – und wo bewusst nicht?
- Welche Teilaufgaben übernimmt KI (z. B. Generierung, Klassifikation, Suche)?
- Wo bleibt menschliche Entscheidung unverzichtbar?
- An welchen Stellen ist Transparenz/Erklärbarkeit wichtig?
- AI-spezifische Risiken (Halluzination, Bias, Datenschutz) und grobe Gegenmaßnahmen.

---

## 8. User Journeys (wichtigste Flows)

Beschreibe 2–4 zentrale Journeys als kurze Story:
- Beispiel:
  - „Firma A kommt mit Problem X, durchläuft Schritt 1–5, erreicht Ergebnis Y.“
  - „Freelancer B nutzt das Produkt, um Z zu erledigen.“
- Fokus auf:
  - Startpunkt (Auslöser),
  - Interaktionen mit dem Produkt,
  - Ergebnis und wahrgenommener Mehrwert.

---

## 9. Geschäftsmodell & Pricing

Wie verdient das Produkt Geld?
- Geschäftsmodell-Typ (z. B. B2B SaaS, Hybrid aus Service + SaaS, Usage-based).
- Pricing-Ideen:
  - Ebenen (Pläne), Metriken (Seats, Projekte, Volumen),
  - Trial-/Freemium-Ansatz (falls sinnvoll).
- Käufer-Persona:
  - Wer unterschreibt den Vertrag? (Rolle im Unternehmen).

---

## 10. Qualitäts- & Reputationsmechanismen

Wie wird sichergestellt, dass das Produkt langfristig Vertrauen aufbaut?
- Mögliche Bewertungs-/Feedbackmechanismen (z. B. Projektbewertungen, NPS).
- Transparenz über Qualität (Dashboards, Statusanzeigen, Health-Checks).
- Schutz vor Missbrauch / „Gaming“ (z. B. Anomalie-Erkennung, Moderation).

---

## 11. Daten, Privacy & Compliance

Welche Daten werden wie verarbeitet?
- Arten von Daten (z. B. personenbezogene Daten, vertrauliche Dokumente).
- Speicherorte, Zugriffe, Verschlüsselung.
- Relevante rechtliche/regulatorische Anforderungen (z. B. DSGVO, branchenspezifische Regeln).
- Prinzipien für Datenschutz & Ethik (z. B. Data Minimization, opt-in/out).

---

## 12. Measurement & Erfolgsmetriken

Was wird gemessen, um Produkt, Technik und Business zu steuern?
- Produkt-Metriken (Aktivität, „Moments of Value“, Funnel).
- Technische Metriken (Fehler, Latenz, Verfügbarkeit, AI-Nutzung).
- Business-Metriken (MRR, Churn, ARPU, Pipeline).
- Wie diese Metriken im Produkt- und Entscheidungsprozess genutzt werden.

---

## 13. Technischer Zielzustand (High-Level-Architektur)

Grobe Architektur-Skizze:
- Frontend/Backend-Technologien,
- Datenhaltung (DB, eventuelle Queues, Suchsysteme),
- AI-Integration (Provider, eigene Modelle, Evals),
- Infrastruktur (Hosting, CI/CD, Observability).

Keine Detailarchitektur, aber klare Leitplanken, was „typisch“ ist.

---

## 14. Betrieb, Support & Continuous Improvement

Wie wird das System im Alltag betrieben und verbessert?
- Betrieb:
  - Monitoring, Alerts, On-Call (falls relevant),
  - Backups, DR-Strategie grob.
- Support:
  - Kommunikationskanäle, Reaktionszeiten, Self-Service-Hilfen.
- Continuous Improvement:
  - Feedback-Kanäle,
  - Umgang mit Änderungen (Feature-Flags, Beta-Programme),
  - Prinzipien für UX-Stabilität (keine ständigen Brüche).

---

## 15. Go-to-Market & erste 90 Tage

Wie sehen die ersten Schritte in den Markt aus?
- Ziel für die ersten 90 Tage (z. B. X Pilotkunden, Y zahlende Kunden).
- Eng definierte Zielkunden und Kanäle (Netzwerk, LinkedIn, Events, Partner).
- Angebot für Early Adopters (z. B. rabattierter Zugang + Feedback).
- Grober 3-Monats-Plan (Monat 1–3: Fokus und Aktivitäten).

---

## 16. Test- und Qualitätsstrategie (High-Level)

Welche Testarten sind für dieses Produkt relevant?
- Produkt-/Value-Tests (kommt es an?).
- Codequalität & funktionale Tests (Unit, Integration, E2E).
- Non-Functional (Performance, Sicherheit, Usability).
- CI-/Release-Tests.
- Für AI-Produkte:
  - Daten-/Modelltests, Guardrails,
  - AI-basierte Szenario-/Simulationstests (optional).

Verweis: Details können in einem separaten Test-Strategie-Dokument ausgearbeitet
werden (z. B. analog zu Abschnitt 21 in `TARGET_STATE_PLATFORM.md`).

