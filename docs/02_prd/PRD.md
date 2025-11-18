# Product Requirements Document (PRD)
# AI-Freelancer-Plattform Deutschland

## Document Info
- **Version**: 1.0 (MVP Lean PRD)
- **Datum**: 27. Oktober 2025
- **Autor**: Klaus Weigele / Codex Agent
- **Status**: Draft → Review

## Document History
| Version | Datum        | Autor         | Änderungen                               |
|---------|--------------|---------------|-------------------------------------------|
| 0.1     | 27.10.2025   | Codex Agent   | Erstfassung (kompakter MVP-Scope)         |
| 1.0     | 27.10.2025   | Codex Agent   | Vollintegration Claude-Code-Inhalte, Backlog & Story Points |

---

## 1. Product Overview

### 1.1 Product Name
**Working Title**: AI-Freelancer-Plattform Deutschland  
**Naming-Optionen**: AI-Match.de, ExpertFlow.de, TalentForge.de, KI-Talente.de  
**Entscheidung**: Nach Phase 03 (Architektur) inkl. Domainprüfung.

### 1.2 Vision
> *„Die fairste und intelligenteste Plattform für KI-Talente in Deutschland.“*

Binnen Tagen statt Monaten erhalten Unternehmen verifizierte AI-Expert:innen, während Freelancer zu fairen Konditionen (2 % Fee) arbeiten und von AI-gestützten Workflows profitieren.

### 1.3 Mission & Problem Statement
- **Firmen** finden keine qualifizierten KI-Spezialisten (149 000 offene IT-Stellen, Talentmangel +50 % seit 2019).  
- **Freelancer** verlieren 10‑16 % Provision und erhalten unpassende Anfragen.  
- **Markt** bietet keine KI-spezifische Plattform mit AI-Features, Compliance-Checks oder fairen Gebühren.

**Lösung**: Kuratierter Matchmaking-Marktplatz mit AI-Briefing, Human-in-the-loop Matching, 2 %-Fee, Compliance-Hub (Scheinselbstständigkeit, Verträge, Zahlungen) und KI-spezifischen Add-ons (Team Assembly, Career Coach, Skill Gap Analyzer).

### 1.4 Target Release
| Phase | Zeitraum | Ziele |
|-------|----------|-------|
| **MVP Build** | Monate 1‑3 | Core-Features (Briefing, Matching, Profile, Contracts, Messaging) |
| **Private Beta** | Monat 4 | 10 Firmen, 30 Freelancer, manuelles Matching |
| **Public Launch** | Monat 5 | Marketing Rollout, 30 Projekte |
| **V1.0** | Monat 6‑12 | AI-Features produktiv, 100 Projekte, 1 Mio. € GMV |

### 1.5 Product Goals (Jahr 1)
1. **Product-Market Fit**: >30 zahlende Firmen, >50 qualifizierte Freelancer, >80 % Trial→Project Conversion.  
2. **Qualität**: AI-Match-Accuracy >85 %, Projekterfolgsrate >90 %, NPS (Freelancer & Firmen) >50.  
3. **Wachstum**: 100 Projekte, 4 Mio. € GMV, 100 000 € Plattformumsatz (2 % Fee).  
4. **Time-to-Match**: <5 Kalendertage vom Briefing bis Vertragsabschluss.  
5. **Marktposition**: #1 KI-Freelancer-Plattform in DACH, 3+ relevante Medienfeatures.

### 1.6 Erfolgsmessung (KPIs)
- Aktiv vermittelte Projekte/Jahr: 100 (Jahr 1), 250 (Jahr 2)  
- Durchschnittliche Besetzungszeit: <5 Tage  
- Freelancer NPS ≥60  
- Take Rate stabil bei 2 %  
- Trial Week Adoption: >70 % der Projekte nutzen Risikofreie Testphase  
- Compliance Incidents: <2 % (auditiert)

---

## 2. Personas & Use Cases

### 2.1 Freelancer Personas

#### F1 – **Max Schreiber**, Senior AI Architect (36)
- **Profil**: 10+ Jahre Software, 4 Jahre AI/ML, Fokus RAG, LangChain, VectorDBs, Python.  
- **Tagessatz**: 1 000 – 1 200 €/Tag, remote-first.  
- **Needs**: Premium-Projekte, faire Provision, schnelle Zahlung, transparente Requirements.  
- **Pain Points**: freelance.de (10 % Fee, unpassende Anfragen), Toptal (30‑50 % versteckte Fee), LinkedIn (Spam, lange Akquise).

#### F2 – **Sara Nguyen**, Emerging AI Engineer (29)
- **Profil**: 5 Jahre Data Science, 2 Jahre LLM Ops, Spezialisierung auf Fine-Tuning, Monitoring.  
- **Tagessatz**: 700 €/Tag.  
- **Needs**: Zugang zu komplexeren Projekten, Upskilling, Coaching.  
- **Pain Points**: Fehlendes Mentoring, Hoffnung auf „Career Coach“ & Skill-Gap-Insights.

#### F3 – **Luca Hoffmann**, AI Apprentice (24)
- **Profil**: Bootcamp-Absolvent, 1 Jahr Praxis.  
- **Needs**: Einstieg über Apprenticeship-Programm, Mentoring, faire Bezahlung.  
- **Pain Points**: Aktuell keine Plattform mit Junior-Fokus, geringe Sichtbarkeit.

### 2.2 Auftraggeber Personas

#### C1 – **Lea Müller**, Head of Engineering (Mid-Market SaaS, 400 MA)
- **Needs**: Besetzung AI-Teams in <5 Tagen, Budgetkontrolle, Compliance-Sicherheit.  
- **Pain Points**: 8‑12 Wochen Hiring, hohe Fees, Risiko Scheinselbstständigkeit.

#### C2 – **David Klein**, CTO Tech-Startup (Series A, 100 MA)
- **Needs**: Schneller Ramp-up für Produkt-Roadmap, variable Kapazitäten, flexible Verträge.  
- **Pain Points**: Kein internes HR, Toptal zu teuer, Upwork unzuverlässig.

#### C3 – **Sophie Berger**, Procurement & Compliance Manager (DAX)
- **Needs**: Vertrags-Templates, Milestone-Abnahmen, Audit Trail, Spend Visibility.  
- **Pain Points**: Manual Workflows, interne Freigaben, Revision.

### 2.3 Primäre Use Cases
| ID | Persona | Use Case | Value |
|----|---------|----------|-------|
| UC-01 | Lea | In <10 Min Projektbriefing erstellen & Shortlist erhalten | Spart Wochen Recruiting |
| UC-02 | Lea | Vertrag & Milestones rechtskonform erstellen | Minimiert Compliance-Risiken |
| UC-03 | Max | Premium-Projekte finden, Trial Week nutzen | Hohe Auslastung & Sicherheit |
| UC-04 | Sophie | Milestones prüfen, Rechnungen freigeben | Auditierbare Prozesse |
| UC-05 | Sara | Skill-Gap & Coaching-Empfehlungen erhalten | Karriereentwicklung |
| UC-06 | Plattform Ops | Freelancer screenen & freischalten | Qualität sichern |

---

## 3. Value Proposition & Differenzierung
- **2 % Plattform-Fee** (statt 10‑16 %).  
- **Hybrid Matching**: AI-Assistent für Briefing + Human-in-the-loop Matching (MVP), später AI-Scores.  
- **Compliance Hub**: Vertragswizard, Statusprüfungen, digitale Signatur, Audit Logs.  
- **AI Talent Ladder**: Apprentice→Expert-Programme, Team Assembly, Career Coach.  
- **Trial Week**: Risikoarme Zusammenarbeit (Storno nach Woche 1).  
- **Schnelle Auszahlung**: ≤7 Tage nach Milestone-Abnahme.

---

## 4. Feature Backlog & Priorisierung

### 4.1 Gesamtübersicht
| ID | Feature | Typ | Priority | Story Points | Status | Bemerkung |
|----|---------|-----|----------|--------------|--------|-----------|
| F-01 | AI Project Builder & Matching | Core | P0 | 8 | MVP | Guided Briefing + Shortlist |
| F-02 | Verifiziertes Freelancer-Profil | Core | P0 | 5 | MVP | Skill Graph, Referenzen |
| F-03 | Contract & Compliance Hub | Core | P0 | 8 | MVP | Vertragsarten, Signatur |
| F-04 | Freelancer Onboarding & Screening | Core | P0 | 5 | MVP | AI Pre-Screen, Interview |
| F-05 | Deal Room & Messaging | Core | P0 | 5 | MVP | Secure Chat, Log |
| F-06 | Milestone & Payment Flow | Core | P0 | 5 | MVP | Abnahmen, Rechnungen, Fee |
| F-07 | Dashboard KPI (Client) | Important | P1 | 3 | V1.0 | Projektstatus, Budget |
| F-08 | AI Talent Team Assembly | Important | P1 | 5 | V1.0 | Ergänzende Rollen |
| F-09 | Trial Week Automatisierung | Important | P1 | 3 | V1.0 | Vertragsoption |
| F-10 | AI Career Coach (Freelancer) | Nice | P2 | 5 | Backlog | Upskilling & Rates |
| F-11 | Integrationen (Jira, Slack) | Nice | P2 | 5 | Backlog | Alerts, Webhooks |
| F-12 | Referral Program | Nice | P2 | 3 | Backlog | Growth |
| F-13 | Mobile App / PWA | Future | P3 | - | Out-of-scope | Post V1.0 |

**MVP Scope**: F‑01 bis F‑06 (≈36 Story Points + zusätzliche 8 für Ops/Admin => Gesamt ≈ 44‑50 SP)  
**V1.0 Erweiterungen**: F‑07 bis F‑09 (≈11 SP)  
**Backlog / Future**: F‑10 ff.

---

## 5. Feature Spezifikationen (P0/P1)

### F‑01: AI Project Builder & Matching
- **Beschreibung**: Geführtes Formular (Problem, Ziel, Scope, Tech-Stack, Budget, Timeline, Remote) inkl. AI-Suggestions & Vorlagen.  
- **Flows**:  
  1. Auftraggeber registriert/verifiziert Unternehmen.  
  2. Project Builder generiert strukturierten Brief.  
  3. Matching-Service (manuell + heuristischer Score) liefert 3‑5 Profile.  
- **Business Value**: Reduziert Time-to-Match, stellt klare Anforderungen sicher.  
- **Abhängigkeiten**: Freelancer Profiles, Matching-Engine, Ops-Team für QA.  
- **Risiken**: Schlechte Input-Qualität → mitigiert durch AI-Suggestions & Pflichtfelder.

### F‑02: Verifiziertes Freelancer-Profil
- Skill-Matrix (Technologien, Frameworks, Level, letzte Nutzung).  
- Referenzprojekte mit Outcome & Tech-Stack.  
- Verifizierungsstatus (ID, Unternehmen, Steuern, Compliance-Check).  
- Badges (Architect, Engineer, Data Scientist, Apprentice).  
- Integration mit Screening-Workflow.

### F‑03: Contract & Compliance Hub
- Vertragsmodelle: Milestone, Sprint, Retainer, Time & Material.  
- Checklisten Scheinselbstständigkeit (z. B. mehrere Auftraggeber, Weisungsfreiheit).  
- Digitale Signatur (z. B. DocuSign/Adobe Sign).  
- Audit Trail (alle Änderungen, Signaturen, Kommentare).  
- Anpassbare Payment Terms (z. B. 7/14 Tage).  
- Integration Payment Provider (Stripe/Mangopay/Lemonway).

### F‑04: Freelancer Onboarding & Screening
- Bewerbung mit Profilangaben, Tagessatz, Branchen, Verfügbarkeit.  
- AI Pre-Screening (CV Parsing, Keyword-Matching, Anomalie-Erkennung).  
- Ops-Review (Interview, Referenzprüfung).  
- Ergebnis: freigeschaltet, zurückgestellt, abgelehnt.

### F‑05: Deal Room & Messaging
- Secure Messaging (verschlüsselt, auditierbar).  
- Meeting-Templates, Checklist für Kick-off.  
- Dokumente (Scopes, SOW) referenzieren (Upload via sichere Lösung Phase 2).  
- Activity Log & Read Receipts (basic).  
- Handshake-Flow (Projektstart, Startdatum).

### F‑06: Milestone & Payment Flow
- Milestone-Planung (Name, Beschreibung, Betrag, Deliverables, Datum).  
- Status: Open → Submitted → Revision → Approved → Paid.  
- Automatische Rechnungserstellung (Freelancer-Branding + Plattform-Fee).  
- Auszahlung ≤7 Tage nach Approval (Payment Provider).  
- Reporting für Kunden (Budget, Burn, Forecast).

### Ergänzende P1-Features
- **F‑07 KPI Dashboard**: Projektsicht (Status, Budget, Zufriedenheit, Risiken).  
- **F‑08 Team Assembly**: Vorschläge für ergänzende Rollen (Data Engineer, MLOps) auf Basis Projektprofil.  
- **F‑09 Trial Week**: Strukturierte Testphase (Scope, Deliverables, Exit-Kriterien).

---

## 6. User Stories (MVP & V1.0)

### 6.1 MVP User Stories (P0)
| US-ID | Persona | Story | Priority | Story Points | Status |
|-------|---------|-------|----------|--------------|--------|
| US-001 | Lea | Projektbriefing erstellen (mit AI-Hilfe) | P0 | 5 | MVP |
| US-002 | Lea | Qualifizierte Shortlist erhalten | P0 | 8 | MVP |
| US-003 | Max | Freelancer-Profil verifizieren | P0 | 5 | MVP |
| US-004 | Sophie | Vertragsmodell & Milestones konfigurieren | P0 | 8 | MVP |
| US-005 | Max | Milestone einreichen & bezahlt werden | P0 | 5 | MVP |
| US-006 | Lea | Im Deal Room kommunizieren & Kick-off planen | P0 | 5 | MVP |
| US-007 | Ops | Freelancer-Screening abschließen | P0 | 4 | MVP |
| US-008 | Ops | Projekte matchen & Shortlist reviewen | P0 | 4 | MVP |

**Total MVP Story Points**: ca. 44‑50 (inkl. technische Tasks)

### 6.2 V1.0 Stories (P1)
| US-ID | Persona | Story | Priority | SP |
|-------|---------|-------|----------|----|
| US-009 | Lea | KPI Dashboard einsehen | P1 | 3 |
| US-010 | Lea | Trial Week konfigurieren | P1 | 3 |
| US-011 | Plattform | Team Assembly Vorschläge erhalten | P1 | 5 |
| US-012 | Sara | Skill-Gap Analyse & Career Coach nutzen | P1 | 5 (P2 optional) |

### 6.3 Beispiel-User Stories mit Akzeptanzkriterien
**US-002 – Shortlist erhalten**  
*Als* Auftraggeber *möchte ich* nach dem Briefing eine qualifizierte Shortlist, *damit* ich schnell Gespräche starten kann.
- [ ] Plattform zeigt min. 3 passende Profile mit Matching-Score & Tagessatz.  
- [ ] Shortlist enthält Begründung (Skills, Projekte, Verfügbarkeit).  
- [ ] Aktion „Gespräch anfragen“ und „Angebot senden“ verfügbar.  
- [ ] Ops kann Vorschläge editieren.  
- [ ] Entscheidung wird geloggt (auditierbar).  
- [ ] Friction-Budget: Anzeige ≤5 Sek.; ≤3 Aktionen bis Deal‑Room‑Öffnung; Abschlussrate ≥70 %.

**US-001 – Projektbriefing erstellen**  
*Als* Head of Engineering *möchte ich* mein Projekt in wenigen Minuten skizzieren, *damit* ich sofort passende Vorschläge erhalte.
- [ ] Abschluss in ≤2 Minuten oder ≤5 Interaktionen.  
- [ ] Minimalfelder: Titel, Ziel, Tech‑Stack‑Tags, Zeitraum/Budget‑Range; rest optional.  
- [ ] AI‑Vorschläge für Scope/ACs; Autosave; Inline‑Validierung.  
- [ ] CTA „Shortlist erzeugen“ direkt nach Abschluss; alternativ „Entwurf speichern“.  
- [ ] Telemetrie: `time_to_brief`, Field‑Drop‑off, Fehlerquote erfasst.

**US-004 – Vertragsmodell & Milestones konfigurieren**  
*Als* Procurement Manager *möchte ich* schnell ein passendes Vertragssetup wählen, *damit* wir rechtssicher starten.
- [ ] Vorauswahl: NDA + Trial‑Week (1 Woche) als editierbares Default‑Bundle.  
- [ ] Vertragsart wählen & ersten Milestone hinzufügen in ≤2 Minuten.  
- [ ] Akzeptanzkriterien/Abnahmeprozess im Wizard enthalten; digitale Signatur vorbereitet.  
- [ ] Audit‑Trail (Erstellung, Änderungen, Signaturen).  
- [ ] Telemetrie: `time_to_contract_ready`, Abbruchpunkte, Fehlfelder.

---

## 7. Functional Requirements
1. **FR-001**: Project Builder validiert Pflichtfelder & Budgetrange, speichert Drafts.  
2. **FR-002**: Matching-Service aggregiert Profile via Skill-Graph (manuell & heuristisch).  
3. **FR-003**: Ops kann Matching-Ergebnisse editieren, kommentieren.  
4. **FR-004**: Freelancer-Verifizierung erfordert manuelle Freigabe nach AI-Pre-Check.  
5. **FR-005**: Vertragswizard generiert PDF + Signatur-Flow.  
6. **FR-006**: Compliance-Checkliste dokumentiert Risikoeinstufung.  
7. **FR-007**: Milestone-Workflow inkl. Benachrichtigungen und Eskalationen.  
8. **FR-008**: Rechnungen berücksichtigen 2 %-Fee inkl. Ausweisung (PDF, Buchhaltung).  
9. **FR-009**: Messaging speichert verkettete Konversationen, verschlüsselt in DB.  
10. **FR-010**: Dashboard aggregiert Projektdaten (SQL Views/Analytics Layer).

---

## 8. Non-Functional Requirements

### 8.1 Performance
- Matching-Antwortzeit: <5 s (bei ≤5 000 Profilen).  
- Dashboard-Load: <2 s (bei ≤1 000 Milestones).  
- API-Endpunkte: p95 <500 ms.

### 8.2 Sicherheit & Compliance
- DSGVO-konforme Speicherung (EU-Region).  
- TLS 1.3, HTTPS only, HSTS.  
- Rollenbasiertes RBAC (Freelancer, Client, Procurement, Ops, Admin).  
- Verschlüsselung ruhender Daten (AES-256), sensible Dateien separat.  
- Logging & Audit Trail (Unveränderbarkeit).  
- Scheinselbstständigkeits-Prüfungen (Checklisten, dokumentierte Entscheidungen).  
- Penetrationstest vor Public Launch.
  
  Policy: Kein Crawling/Text-&-Data‑Mining (TDM) externer Projektbörsen, kein Screen‑Scraping und keine Übernahme fremder Inhalte. Nur First‑Party‑Daten (auf unserer Plattform) oder explizit autorisierte Integrationen/Feeds.

  Datenschutz & Rechtstexte: Siehe `docs/02_prd/legal-texts.md` (Entwurf). Kernpunkte:
  - Rechtsgrundlage: Art. 6 Abs. 1 lit. f DSGVO; Veröffentlichung nur aggregiert/anonymisiert; keine Namen/Logos/IDs/Originaltexte.
  - Rohdaten‑Retention für Statistikaufbereitung max. 90 Tage; aggregierte, nicht‑personenbeziehbare Werte dürfen länger vorgehalten werden.
  - Widerspruchsrecht gem. Art. 21 DSGVO (via Kontoeinstellungen oder E‑Mail an datenschutz‑Kontakt).

### 8.3 Skalierbarkeit & Architektur
- Modularer Aufbau (Next.js App Router, Backend-Services, Worker für Matching).  
- Matching-Service vorbereitet für Vektor-Datenbank (Pinecone/Weaviate) in V1.0.  
- Event-basierte Kommunikation (Milestone-Events, Notifications).  
- Infrastruktur: AWS (ECS/Fargate, RDS Postgres, S3, CloudFront), CI/CD via GitHub Actions.

### 8.4 Usability & Accessibility
- Responsive (Desktop, Tablet, Mobile Web).  
- WCAG 2.1 AA (Kontrast, Keyboard-Navigation).  
- Deutsch als Primärsprache, englische UI später (P2).  
- Geführte Onboarding-Flows, Tooltips, Inline-Validierung.

### 8.5 UX-Friction & Instrumentation
- Friction‑Budget je Kernflow: Abschluss in ≤2 Minuten oder ≤5 Interaktionen; Ziel‑Abschlussrate ≥70 %.  
- Instrumentation: `time_to_first_action`, `time_to_shortlist`, `field_dropoff`, `completion_rate`.  
- Optimistic UI, Autosave, Prefetching; klare Erfolgs‑/Fehlerzustände.

---

## 9. User Flows

### Flow 1: Projekt anlegen & Match erhalten
1. Client registriert sich, verifiziert Unternehmen (USt-ID, HR-Kontakt).  
2. Project Builder → AI-Suggestions → Review → Submit.  
3. Matching-Service erstellt Shortlist → Ops validiert → Client erhält Benachrichtigung.  
4. Client lädt ausgewählte Freelancer in Deal Room ein.  
5. Trial Week optional → Vertragsdetails finalisieren → digitale Signatur.

### Flow 2: Freelancer Onboarding
1. Bewerbung (Skills, CV, Tagessatz, Branchen).  
2. AI Pre-Screen (Keyword-Score, Anomalien).  
3. Ops Interview + Referenzprüfung.  
4. Profil freigeschaltet → erscheint in Talentpool.  
5. Erhält Projektanfragen → Deal Room → Start.

### Flow 3: Milestone Abrechnung
1. Freelancer markiert deliverable als „Submitted“.  
2. Client reviewt innerhalb 5 Tagen (Approve/Revision).  
3. Plattform generiert Rechnung (PDF, Buchung).  
4. Payment Provider zahlt aus (minus Fee).  
5. Dashboard aktualisiert Budget & Status.

---

## 10. MVP Definition & Release Plan

### 10.1 In Scope (MVP)
- F‑01 bis F‑06 (Project Builder, Matching, Profile, Contracts, Messaging, Milestones).  
- Admin/Ops-Backoffice (Basic Dashboard, Matching Console).  
- Manuelles Matching (Human-led, AI-Assistance optional).  
- Payment Flow via Provider (Payout ≤7 Tage).  
- Basic Reporting (Projektstatus, Budget).

### 10.2 Out of Scope (MVP)
- Automatisierte AI-Matching-Scores (Ranking) – geplant für V1.0.  
- Integrationen (Jira, Slack, Calendar).  
- Rating/Review-System.  
- File-Sharing im Chat.  
- Escrow & Auto-Payments.  
- Mobile Apps & PWA.  
- Mehrsprachigkeit (EN).  
- Advanced Analytics/Insights.  
- Referral & Loyalty Programme.  
- Recruiting für Festanstellungen.
  
  Recht/Quellen: Externes Crawling/TDM/Screen‑Scraping von Projektbörsen (freelancermap, freelance.de, GULP, Malt, projektwerk etc.) ist ausgeschlossen.

### 10.4 Rechtliche Hinweise (MVP)
- Aggregations‑/Statistikfunktion basiert ausschließlich auf Plattform‑Eigeninhalten und erfolgt anonymisiert/aggregiert (keine Personen-/Firmendaten, keine Originaltexte).
- Entsprechende Passagen in Datenschutzerklärung und AGB werden gemäß `docs/02_prd/legal-texts.md` umgesetzt.

### 10.3 MVP Timeline (Sprints à 2 Wochen)
| Sprint | Fokus | Stories |
|--------|-------|---------|
| S1 | Setup & Auth, Datenmodelle | US-003, US-007 (Teil) |
| S2 | Project Builder & Matching Backend | US-001, US-008 |
| S3 | Freelancer Profiles & Screening | US-003, Ops Funktionen |
| S4 | Contracts, Compliance | US-004 |
| S5 | Deal Room, Messaging | US-006 |
| S6 | Milestones & Payments | US-005 |
| S7 | Hardening & Private Beta | QS, Security, Docs |

---

## 11. Datenmodell (High Level)
- **User** (id, role, name, email, verified, company_id)  
- **Company** (id, name, industry, size, compliance_status)  
- **FreelancerProfile** (user_id, bio, skills[], experience_years, availability, rate, badge, verification_status)  
- **Skill** (id, name, category, embedding_vector?)  
- **Project** (id, company_id, title, scope, tech_stack[], budget_range, status, confidentiality)  
- **Match** (id, project_id, freelancer_id, score, status, notes)  
- **Contract** (id, project_id, freelancer_id, type, start_date, end_date, fee_percent, signed_at)  
- **Milestone** (id, contract_id, title, amount, due_date, status, revision_count)  
- **Invoice** (id, milestone_id, amount_net, fee_amount, issue_date, payout_date, payout_status)  
- **Message** (id, room_id, sender_id, content, metadata, created_at)  
- **AuditLog** (id, entity, entity_id, action, actor_id, timestamp, payload)

---

## 12. API Endpunkte (High Level)
- `POST /api/auth/register` – Registrierung (Freelancer, Client)  
- `POST /api/auth/login` – Login  
- `POST /api/projects` – Projektbriefing speichern  
- `GET /api/projects/{id}/matches` – Shortlist abrufen  
- `POST /api/projects/{id}/matches/{freelancerId}/invite` – Einladung versenden  
- `POST /api/freelancers` – Bewerbungsprozess starten  
- `PATCH /api/freelancers/{id}/status` – Verifizierung updaten (Admin/Ops)  
- `POST /api/contracts` – Vertrag anlegen (inkl. Trial Option)  
- `POST /api/contracts/{id}/sign` – Signatur (Client/Freelancer)  
- `POST /api/milestones/{id}/submit` – Milestone einreichen  
- `POST /api/milestones/{id}/approve` – Milestone abnehmen  
- `POST /api/milestones/{id}/reject` – Revision anfordern  
- `GET /api/dashboard` – KPIs (Client)  
- `POST /api/messages` – Nachricht senden  
- `GET /api/messages/{roomId}` – Verlauf laden  
- `GET /api/admin/pipeline` – Ops Dashboard (Matches, Onboarding)

---

## 13. Assumptions, Risks & Dependencies

### 13.1 Annahmen
- Unternehmen akzeptieren Plattform-Rechnungen (2 %-Fee) und 7‑Tage Auszahlung.  
- Erste 50 Projekte können manuell gematcht werden (Ops-Kapazität verfügbar).  
- Payment Provider (Stripe, Lemonway) unterstützt Treuhand & Compliance in DE.  
- Freelancer liefern verifizierbare Referenzen.  
- KI-Nachfrage bleibt stabil bzw. steigt (Post-ChatGPT-Boom).

### 13.2 Risiken (Top 3 aus Risk Assessment)
- **R1: Scheinselbstständigkeit** – Mitigation: Fachanwalt, Checklisten, Vertragsgestaltung, Schulungen.  
- **R2: Wettbewerber senkt Provision** – Mitigation: AI-Differenzierung, Community, schnelle Markteinführung.  
- **R3: Matching Qualität** – Mitigation: Human-in-the-loop im MVP, Feedback-Schleifen, Score-Engine V1.0.

### 13.3 Abhängigkeiten
- Payment Provider Onboarding (KYC, Compliance).  
- Juristische Beratung (AGB, Verträge, Datenschutz).  
- Verfügbarkeit von AI/Embedding-APIs (Anthropic/OpenAI/Pinecone).  
- Marketing/Vertrieb für Pilotkunden.

### 13.4 Offene Fragen
- [ ] Welcher Payment Provider (Stripe, Mangopay, Lemonway) erfüllt Treuhand-Anforderungen?  
- [ ] Wie wird das Referral-Programm strukturiert (Provisionierung, Tracking)?  
- [ ] Welche Gesellschaftsform (UG/GmbH) & Versicherungen (PI, Cyber) sind Pflicht vor Launch?  
- [ ] Welche Datenhaltung ist für Compliance-Checks notwendig (z. B. Speicherdauer)?

---

## 14. Appendices & Referenzen
- **Business Case**: `/Users/klausweigele/softwareprojekte_claude/freelancer/BUSINESS_CASE.md`  
- **Markt- & Wettbewerbsanalyse**: `docs/01_business-idea/competitor-analysis.md`  
- **Risk Assessment**: (Phase 01 Deliverable)  
- **Weitere Recherchen**: folgen unter `docs/01_business-idea/`  
- **Design/Wireframes**: werden in Phase 04 (UX) erstellt (`docs/04-ux/`).

---

## 15. Sign-off & Next Steps
- ✅ Business Idea validiert (Phase 01)  
- ✅ PRD erstellt & mit Claude-Code-Version harmonisiert  
- ⏳ Review/Approval (Selbstreview + ggf. Stakeholder)  
- ▶️ Nächste Phase: `03-architecture` (Tech Stack, Datenmodell, Systemdesign, Ops Playbooks)  
- 📌 Nach Review `support/project-context-manager` & `support/quality-gate-checker` ausführen.

**Status**: PRD draft ready for review.  
**Geplanter Review-Termin**: 28. Oktober 2025.  
**Freigabe erforderlich durch**: Product Owner (du) → danach Phase 03 starten.
