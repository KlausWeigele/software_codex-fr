# Zielbild: AI-Dokumentationsassistent für ambulante Pflege

Status: Entwurf v0.1  
Arbeitsname: „PflegeDoc AI“

Zweck: Zielzustand für ein SaaS-Produkt, das ambulante Pflegedienste bei der
rechtssicheren, schnellen Dokumentation mit Hilfe von KI unterstützt.

---

## 1. Produkt-Vision

- Pflegekräfte verbringen deutlich weniger Zeit mit Dokumentation und mehr Zeit
  bei den Menschen.
- Dokumentation ist rechtssicher, konsistent und MDK-/Kassen-konform, ohne
  dass Pflegekräfte Paragraphen kennen müssen.
- Die Lösung fügt sich in den Arbeitsalltag ambulanter Pflege „wie ein
  Teammitglied“ ein: per Sprache erfassen, KI strukturiert und die Pflegekraft
  gibt nur frei.

---

## 2. Zielgruppen & Rollen

**Primäre Zielgruppe**
- Ambulante Pflegedienste, Sozialstationen in Deutschland.

**Rollen**
- Pflegekräfte:
  - erfassen Verlaufsdokumentation, Maßnahmen, Beobachtungen, Leistungsnachweise.
- Pflegedienstleitung / Qualitätsbeauftragte:
  - sind verantwortlich für Vollständigkeit, Qualität und MDK-Konformität.
- Inhaber / Geschäftsführung:
  - tragen wirtschaftliche Verantwortung, unterschreiben Verträge.

**Jobs-to-be-done**
- Pflegekräfte:
  - „Ich möchte am Ende der Tour nicht noch 1–2 Stunden Formulare ausfüllen
    müssen.“
- Pflegedienstleitung:
  - „Ich möchte sicher sein, dass unsere Doku bei Prüfungen nicht auseinander-
    genommen wird.“
- Inhaber:
  - „Ich möchte mehr Patienten versorgen können, ohne mein Team zu überlasten.“

---

## 3. Leitprinzipien des Produkts

- **Care-first:** Immer zuerst an den Alltag der Pflegekräfte denken, dann an
  Technik.
- **Super-simpel:** So wenig UI wie möglich, klare Sprache, große Buttons,
  handschuhtauglich.
- **AI-first, human-in-the-loop:** KI schlägt Doku vor, Pflegekraft bestätigt/
  korrigiert. Kein „Blackbox-Autopilot“.
- **Rechtssicher & nachvollziehbar:** Jeder Eintrag ist im Zweifel
  erklärbar/prüfbar (MDK, Kasse, Gericht).
- **Offline-fähig & robust:** Touren dürfen nicht an Funklöchern scheitern.
- **Liberal & anreizbasiert:** System macht es *attraktiv*, sauber zu
  dokumentieren (Weniger Stress, bessere Übersicht), keine Gängelung.

---

## 4. Problem & Pain Points

1. **Dokumentationswahnsinn**
   - 30–40 % Arbeitszeit gehen für Doku drauf; häufig am Ende der Schicht unter
     starker Müdigkeit.
   - Risiko von Fehlern, Lücken, nachträglichen „Gedächtnisprotokollen“.

2. **Regulatorische Komplexität**
   - SIS, Expertenstandards, Abrechnungscodes (SGB XI/V) sind komplex.
   - Pflegekräfte müssen sich auf Menschen konzentrieren, nicht auf Codierungen.

3. **Alte, unergonomische Systeme**
   - Diktiergeräte, komplexe Pflegesoftware, Papier → später digitalisieren.
   - Eingaben sind langsam, mühsam, oft nur am Büro-PC möglich.

4. **Angst vor Prüfungen**
   - MDK-/Kassenprüfungen erzeugen hohen Stress.
   - Dokumentation ist uneinheitlich, schwer nachzuvollziehen.

5. **Fachkräftemangel**
   - Jeder ineffiziente Dokumentationsprozess verschärft den Personalmangel.

Heutige Workarounds:
- Diktieren auf Band/Smartphone, Freitext in bestehender Software,
  nachträgliche Erinnerungseinträge, Überstunden, unentgeltliche Mehrarbeit.

Schwächen:
- Fehleranfällig, ineffizient, schlecht strukturiert, psychisch belastend.

---

## 5. Wertversprechen & Differenzierung

**Kernversprechen**
- „Halbiere deine Dokumentationszeit ohne Qualitätsverlust.“
- „Komm entspannter durch MDK-/Kassenprüfungen.“
- „Mehr Zeit mit Patienten, weniger Zeit auf dem Sofa mit Formularen.“

**Differenzierung**
- Spezifischer Fokus auf ambulante Pflege (nicht „alle Gesundheitsbereiche“).
- Starke Sprach-/Mobile-UX + KI-Assistenz statt klassischer Formularwüsten.
- Klarer MDK-/Abrechnungs-Fokus, nicht nur „Notizen-App“.

---

## 6. Kernfunktionen (Version 1)

1. **Sprachbasierte Verlaufsdokumentation**
   - Pflegekraft spricht direkt nach dem Besuch Stichpunkte ein.
   - KI erzeugt strukturierten Verlaufsbericht + Vorschlag für relevante Felder.

2. **Strukturierung in SIS-/Doku-Felder**
   - Mapping von Freitext auf vordefinierte Felder (z. B. Ressourcen, Probleme,
     Maßnahmen).

3. **Abrechnungs-Hinweise (light)**
   - Erste Version nur als „Hinweis“, keine automatische Abrechnung:
   - z. B. „Dies könnte Leistung X/Y sein – bitte prüfen.“

4. **Qualitäts-Check & Erinnerungen**
   - Hinweise auf fehlende Angaben (z. B. Datum, Vitalwerte, Schmerzskala).

5. **Export / Schnittstelle**
   - PDF-Export + strukturierter Text für Copy&Paste in bestehende Software.
   - Später: direkte API-Integration zu ausgewählten Pflegesoftware-Anbietern.

Non-Goals in V1:
- Vollständiger Ersatz der Primär-Pflegesoftware,
- komplexe Dienst-/Tourenplanung,
- automatisierte Abrechnung.

---

## 7. Rolle von KI

- **Erfassung:** Speech-to-Text in deutscher Sprache, angepasst an Pflegekontext.
- **Verstehen:** NLU, um klinisch/pflegerisch relevante Informationen zu
  extrahieren.
- **Strukturierung:** Mapping auf Doku-Schemata (SIS, Maßnahmen, Beobachtungen).
- **Qualitätssicherung:** Hinweise auf Inkonsistenzen, fehlende Angaben,
  Plausibilitätschecks.

Grenzen:
- Pflegekraft bleibt fachlich verantwortlich, prüft und bestätigt.
- Keine „autonome“ Dokumentation ohne menschlichen Blick.

Risiken & Gegenmaßnahmen:
- Halluzination → starke Constraints, Vorlagen, Post-Editing Pflicht.
- Verwechslung von Patienten → klare Patientenauswahl im UI, keine reine
  Stimmerkennung.
- Datenschutz → Verschlüsselung, möglichst On-Device/Edge-Lösungen, deutsche/
  EU-Cloud-Anbieter, klarer Auftragsverarbeitungsvertrag.

---

## 8. User Journeys (wichtigste Flows)

**Journey 1: Dokumentation nach Hausbesuch**
- Pflegekraft schließt Besuch ab, öffnet App, wählt Patient.
- Spricht 30–60 Sekunden Bericht („Heute war…“).
- KI erzeugt strukturierte Dokumentation.
- Pflegekraft korrigiert/kürzt, bestätigt, fertig.

**Journey 2: Prüfungsvorbereitung**
- Pflegedienstleitung filtert Dokumentation für einen Zeitraum/Patienten.
- System zeigt Vollständigkeitsstatus + Auffälligkeiten.
- Leitung geht mit Stichwortliste in Prüfung; fühlt sich vorbereitet.

**Journey 3: Onboarding neuer Pflegekraft**
- Neue Pflegekraft sieht Beispiel-Einträge + kurze How-tos.
- KI gibt Feedback bei ersten Einträgen („Fehlt noch…“).

---

## 9. Geschäftsmodell & Pricing

- Typ: B2B SaaS.
- Pricing-Ideen:
  - pro aktivem Pflegekraft-Account/Monat,
  - Staffelpreise nach Größe des Pflegedienstes.
- Trial:
  - 30 Tage kostenlos, begrenzte Patientenzahl,
  - oder „bis X Dokumentationen“.
- Käufer-Persona:
  - Inhaber / Geschäftsführung,
  - Pflegedienstleitung mit Budgetverantwortung.

---

## 10. Qualitäts- & Reputationsmechanismen

- Qualitätsmetriken:
  - durchschnittliche Dokumentationszeit vor/nach Einsatz,
  - Vollständigkeit/Fehlerrate (z. B. aus internen Audits),
  - Zufriedenheit der Pflegekräfte.
- Feedback:
  - Einfache In-App-Feedbackfunktion („Das war hilfreich / nicht hilfreich“),
  - strukturierte Postmortems nach MDK-Prüfungen („Wie hat das Tool geholfen?“).
- Reputation:
  - Fallstudien mit anonymisierten Daten,
  - Empfehlungen von Pflegedienstleitungen.

---

## 11. Daten, Privacy & Compliance

- Datenarten:
  - hochsensible Gesundheitsdaten, personenbezogene Daten, Leistungsdaten.
- Anforderungen:
  - strenge DSGVO-Konformität,
  - TOMs, Verschlüsselung in Ruhe und Transport,
  - klarer AV-Vertrag, Datenlokation in EU,
  - Logging & Zugriffskontrollen.
- Besonderheiten:
  - mögliche Einbindung von Betriebsrat/Datenschutzbeauftragten,
  - ggf. medizinrechtliche Beratung (Haftung).

---

## 12. Measurement & Erfolgsmetriken

- Produkt:
  - Anzahl dokumentierter Einsätze pro Pflegekraft/Tag,
  - durchschnittliche Zeit pro Dokumentation,
  - Nutzungsrate (wie oft wird die App genutzt, vs. altes System).
- Business:
  - MRR, Churn, durchschnittlicher Umsatz pro Pflegedienst,
  - Anzahl mitlaufender Pilotkunden, Net Promoter Score der Leitungen.
- Impact:
  - subjektive Entlastung der Pflegekräfte,
  - Time-to-Document nach Einsatz (weniger „Abend-Berge“).

---

## 13. Technischer Zielzustand (High-Level-Architektur)

- Client:
  - Mobile App (Android, ggf. iOS) + Web-App für Leitung.
- Backend:
  - API (REST/tRPC), Auth, Tenant-Verwaltung, Audit-Logs.
- Datenbank:
  - PostgreSQL, strikte Mandantentrennung.
- AI-Schicht:
  - Speech-to-Text (deutsch), Domain-NLU, Prompt-/RAG-Layer,
  - eventuell eigene Modelle oder feinjustierte Provider.
- Infrastruktur:
  - Cloud (EU), Docker/Kubernetes oder managed Plattform,
  - CI/CD mit automatisierten Tests und Deployments.

---

## 14. Betrieb, Support & Continuous Improvement

- Betrieb:
  - Monitoring von Latenz, Fehlern, Speech-/AI-Limits,
  - Backups, DR-Pläne (besonders für Doku-Daten).
- Support:
  - Niedrigschwelliger Support-Kanal (Telefon/WhatsApp/Chat),
  - einfache Hilfetexte + kurze Videos.
- Continuous Improvement:
  - Feedback-Auswertung,
  - AI-Simulationen mit synthetischen Pflege-Szenarien,
  - vorsichtige UI-Änderungen (Stabilität für gestresste Nutzer).

---

## 15. Go-to-Market & erste 90 Tage (Skizze)

- Ziel:
  - 3–5 Pilot-Pflegedienste,
  - 20–50 aktive Pflegekräfte, die das System im Alltag nutzen.
- Kanäle:
  - direkte Ansprache von Pflegedienstleitungen,
  - Kontakte über Verbände, persönliche Netzwerke,
  - ggf. Kooperation mit Pflegesoftware-Anbieter als Add-on.
- Angebot für Early Adopters:
  - stark rabattierter oder kostenloser Pilot gegen strukturiertes Feedback,
  - Unterstützung bei Prüfungen als Mehrwert.

---

## 16. Test- und Qualitätsstrategie (High-Level)

- Produkt-/Value-Tests:
  - begleitete Tests mit Pflegekräften im Feld,
  - qualitative Interviews nach Testphasen.
- Funktionale Tests:
  - Unit-/Integrationstests für Doku-Logik,
  - E2E-Flows (Sprache → Doku → Export).
- Non-Functional:
  - Lasttests (viele Einsätze gleichzeitig),
  - Offline-/Reconnect-Tests,
  - Security- und Pen-Tests.
- AI-Tests:
  - Evaluationssets für typische Dokumentationsszenarien,
  - Bias/Risiko-Checks (keine gefährlichen Interpretationen).
- Simulation:
  - AI-Agents, die typische Touren und Doku-Situationen nachspielen
    (Ergänzung zu echten Nutzern).

